# jquery-easyui-extensions
Extensions(Helpers) for JQuery Easyui

## I. Install

    ```
    npm i jquery-easyui-extensions
    ```
    or
    ```
    yarn add jquery-easyui-extensions
    ```

## II. Usage

1. Create from Smfony Not Mapped Form Field

    ```
    require( 'jquery-easyui-extensions/EasyuiCombobox.css' );
    import { EasyuiCombobox } from 'jquery-easyui-extensions/EasyuiCombobox.js';
    
    $( function()
    {
        let categorySelector    = "#product_form_categories";
        let selectedCategories  = JSON.parse( $( '#product_form_productCategories').val() );
        EasyuiCombobox( $( categorySelector ), {
            required: true,
            multiple: true,
            checkboxId: "product_category",
            values: selectedCategories,
            debug: false
        });
    });
    ```
