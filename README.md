Aijko_WidgetImageChooser
========================

## Branches

* master => stable version of this extension (tested with EE 1.12.0.2)
* develop => development version

## About this extension

Aijko_WidgetImageChooser introduces a new field type **widgetimagechooser/chooser** in the widget declaration to use the
standard Magento image chooser in widgets as well.

## How-To

Just use **widgetimagechooser/chooser** as the type when declaring the widget:

    <image>
        <label>Image</label>
        <type>widgetimagechooser/chooser</type>
    </image>


Example widget.xml:

    <?xml version="1.0"?>
    <widgets>
        <widget_sample type="custom/widget" translate="label description" module="your_custom">
            <name>Test Widget</name>
            <parameters>
                <title>
                    <label>Title</label>
                    <required>1</required>
                    <visible>1</visible>
                    <type>text</type>
                    <sort_order>10</sort_order>
                </title>
                <text>
                    <label>Text</label>
                    <required>1</required>
                    <visible>1</visible>
                    <type>textarea</type>
                    <sort_order>20</sort_order>
                </text>
                <image>
                    <label>Image</label>
                    <required>1</required>
                    <visible>1</visible>
                    <type>widgetimagechooser/chooser</type>
                    <sort_order>30</sort_order>
                </image>
            </parameters>
        </widget>
    </widgets>