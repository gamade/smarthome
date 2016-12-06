# My Plugin

# Requirements

List the requirements of your plugin. Does it need special software or hardware?

## Supported Hardware

* list
* the
* supported
* hardware

# Configuration

* Send command "/newbot" to "BotFather" in order to create your new bot
* you will asked for a bot name and unique username 
* BotFather will send you a token (=shard secred) you will need for plugin registration
* configure some bot details starting by sending "/mybots" to BotFather

## plugin.conf

Please provide a plugin.conf snippet for your plugin with ever option your plugin supports. Optional attributes should be commented out.

<pre>

[telegram]
        class_name = Telegram
        class_path = plugins.telegram
        token = "123456789:BBCCfd78dsf98sd9ds-_HJKShh4z5z4zh22"
        trusted_chat_ids = 123456789,9876543210

</pre>

Please provide a description of the attributes.
This plugin needs an host attribute and you could specify a port attribute which differs from the default '1010'.

## items.conf

List and describe the possible item attributes.

### my_attr

Description of the attribute...

### my_attr2

### Example

Please provide an item configuration with every attribute and usefull settings.

<pre>
# items/my.conf

[someroom]
    [[mydevice]]
        type = bool
        my_attr = setting
</pre>

## logic.conf
If your plugin support item triggers as well, please describe the attributes like the item attributes.


# Methodes
If your plugin provides methods for logics. List and describe them here...

## method1(param1, param2)
This method enables the logic to send param1 and param2 to the device. You could call it with `sh.my.method1('String', 2)`.

## method2()
This method does nothing.
