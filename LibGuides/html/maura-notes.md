The templates should likely change once the system-wide header/footer are updated (because we would then want to use the system-wide headers and footers instead of overriding them)

```
<body class="s-lib-public-body">
    {{skip_link}}
    {{obsolete_browser_alert}}

    <!-- BEGIN: Page Header -->
    {{public_header}}
    <!-- END: Page Header -->

    ** other code **

    <!-- BEGIN: Custom Footer -->
    {{public_footer}}
    <!-- END: Custom Footer -->
</body>
```

Would also want to remove ```body.hl__template``` from beginning of all header/footer content, but make sure that there is something like .hl__header and .hl__footer still present (so as not to disrupt other groups' header/footer customizations)

Could also use this opportunity to create a template for how to create own similar header with their school logo in the top right + update the background color.

Add favicon?

If you don't want our footer, can you include the system default one? Try adding this code into the footer section:

```
<!-- BEGIN: Page Footer -->
    {{system_footer}}
<!-- END: Page Footer -->
```