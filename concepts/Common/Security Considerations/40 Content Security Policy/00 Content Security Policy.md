[Content Security Policy](https://developer.mozilla.org/ru/docs/Web/HTTP/CSP) (CSP) is a security feature that helps detect and mitigate certain types of attacks, such as clickjacking, cross-site scripting (XSS), and other malicious code injection attacks. The impact of such attacks varies but can include data theft, page spoofing, malware distribution, site defacement, etc. It is important to ensure that DevExtreme UI components are compatible with CSP.

If you want to apply CSP rules, define a `<meta>` tag and configure your policy in the following manner:

    <!--HTML-->
    <meta
        http-equiv="Content-Security-Policy"
        content="default-src 'self'; img-src https://*; child-src 'none';" />
