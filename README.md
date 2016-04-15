KMadera_Magento1Xsds
==================================

This module provides XSDs for Magento 1 to enable IDE auto-completion and structure validation.

## Installation
Install this module into your Magento project via composer, then enable it in each of your config xml files.

```
composer install kirkmadera/magento1-xsds
```

## Supported configuration files

### Module Config XML
Add this to your config.xml files in the root `<config>` node
```
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="../../../../../code/community/KMadera/Magento1Xsds/etc/schema/config.xsd"
```

### Layout XML
Add this to your config.xml files in the root `<config>` node
```
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="../../../../../code/community/KMadera/Magento1Xsds/etc/schema/layout.xsd"`\
```

## Known Issues
Magento 1 uses custom node names which makes it difficult to write XSDs for. I have not yet found a way
to state the structure for all nodes at a certain child level of another node, regardless of the name.
This would make XSDs possible for many other config files in Magento 1 like system.xml, adminhtml.xml, widget.xml, etc.

## Please contribute!
I'd like to have a more complete list of XSDs, but are either blocked or have not found the time to sdo so yet.
