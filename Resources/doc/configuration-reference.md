Full default configuration
==========================

```yaml
fos_rest:
    param_fetcher_listener:  false
    cache_dir:            %kernel.cache_dir%/fos_rest
    allowed_methods_listener:  false
    routing_loader:
        default_format:       ~
    service:
        router:               router
        templating:           templating
        serializer:           jms_serializer.serializer
        view_handler:         fos_rest.view_handler.default
    serializer:
        version:              ~
        groups:               []
    view:
        default_engine:       twig
        force_redirects:

            # Prototype
            name:                 []
        mime_types:

            # Prototype
            name:                 []
        formats:

            # Prototype
            name:                 []
        templating_formats:

            # Prototype
            name:                 []
        view_response_listener:  false
        failed_validation:    400
    exception:
        codes:

            # Prototype
            name:                 []
        messages:

            # Prototype
            name:                 []
    body_listener:
        decoders:

            # Prototype
            name:                 []
    format_listener:
        default_priorities:

            # Defaults:
            - html
            - */*
        prefer_extension:     true
        fallback_format:      html
```

