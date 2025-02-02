DevExtreme Vue components are supplied with TypeScript declarations. Strict typing allows you to catch bugs at earlier stages and use features like code completion and automated refactoring.

The following code shows an example of using TypeScript with DevExtreme components in a Vue application:

    <!-- tab: App.vue -->
    <template>
        <div>
            <DxList :items="items" ref="list">
                <template #item="{data}">
                    <Item :text="data.text" />
                </template>
            </DxList>
        </div>
    </template>

    <script lang='ts'>
    import { Component, Vue } from 'vue-property-decorator';
    import { DxList } from 'devextreme-vue/list';
    import Item from './components/Item.vue';
    
    interface IListItemProps {
        text: string;
    }
    
    @Component({
        components: {
            DxList,
            Item
        }
    })

    export default class App extends Vue {
        public $refs: Vue['$refs'] & {
            list?: DxList,
        } = {};
        
        public items: IListItemProps[] = [
            { text: 'Item 1' },
            { text: 'Item 2' },
            { text: 'Item 3' }
        ];
    }
    </script>

    <!-- tab: Item.vue -->
    <template>
        <div @click="addCounter">
            {{text}} was clicked {{counter}} times
        </div>
    </template>
    
    <script lang='ts'>
    import { Component, Prop, Vue } from 'vue-property-decorator';  

    @Component
    export default class Item extends Vue {
        @Prop() public text!: string;
        public counter: number = 0;
        public addCounter() {
            this.counter = this.counter + 1;
        }
    }
    </script>

To import component-specific types, use the `DxComponentTypes` declaration where `Component` is the component name:

    <!-- tab: App.vue -->
    <template>
        <DxDateBox :type="dateType" />
    </template>

    <script setup lang="ts">
    import DxDateBox, { DxDateBoxTypes } from "devextreme-vue/date-box";

    const dateType: DxDateBoxTypes.DateType = "datetime";
    </script>

#####See Also#####
- <a href="https://v3.vuejs.org/guide/typescript-support.html" target="_blank">TypeScript Support in Vue Documentation</a>

[tags] vue