##### [load_appium_txt](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L72) 

> def self.load_appium_txt opts={}

Load appium.txt (toml format)
the basedir of this file + appium.txt is what's used

```
[caps]
app = "path/to/app"

[appium_lib]
port = 8080
```

:app is expanded
:require is expanded
all keys are converted to symbols

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - file: '/path/to/appium.txt', verbose: true

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[hash] the symbolized hash with updated :app and :require keys

--

##### [symbolize_keys](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L142) 

> def self.symbolize_keys hash

convert all keys (including nested) to symbols

based on deep_symbolize_keys & deep_transform_keys from rails
https://github.com/rails/docrails/blob/a3b1105ada3da64acfa3843b164b14b734456a50/activesupport/lib/active_support/core_ext/hash/keys.rb#L84

--

##### [promote_singleton_appium_methods](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L155) 

> def self.promote_singleton_appium_methods modules

if modules is a module instead of an array, then the constants of
that module are promoted on.
otherwise, the array of modules will be used as the promotion target.

--

##### [promote_appium_methods](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L195) 

> def self.promote_appium_methods class_array

Promote appium methods to class instance methods

To promote methods to all classes:

```ruby
Appium.promote_appium_methods Object
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Class>] class_array - An array of classes

--

##### [global_webdriver_http_sleep](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def global_webdriver_http_sleep

The amount to sleep in seconds before every webdriver http call.

--

##### [global_webdriver_http_sleep=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def global_webdriver_http_sleep=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [caps](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def caps

The amount to sleep in seconds before every webdriver http call.

--

##### [caps=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def caps=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [custom_url](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def custom_url

The amount to sleep in seconds before every webdriver http call.

--

##### [custom_url=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def custom_url=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [export_session](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def export_session

The amount to sleep in seconds before every webdriver http call.

--

##### [export_session=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def export_session=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [default_wait](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def default_wait

Returns the default client side wait.
This value is independent of what the server is using

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Integer] 

--

##### [default_wait=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def default_wait=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [last_waits](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def last_waits

The amount to sleep in seconds before every webdriver http call.

--

##### [last_waits=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def last_waits=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [sauce_username](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def sauce_username

The amount to sleep in seconds before every webdriver http call.

--

##### [sauce_username=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def sauce_username=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [sauce_access_key](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def sauce_access_key

The amount to sleep in seconds before every webdriver http call.

--

##### [sauce_access_key=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def sauce_access_key=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [appium_port](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def appium_port

The amount to sleep in seconds before every webdriver http call.

--

##### [appium_port=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def appium_port=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [appium_device](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def appium_device

The amount to sleep in seconds before every webdriver http call.

--

##### [appium_device=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def appium_device=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [appium_debug](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def appium_debug

The amount to sleep in seconds before every webdriver http call.

--

##### [appium_debug=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L228) 

> def appium_debug=(value)

The amount to sleep in seconds before every webdriver http call.

--

##### [initialize](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L259) 

> def initialize opts={}

Creates a new driver

```ruby
require 'rubygems'
require 'appium_lib'

# platformName takes a string or a symbol.

# Start iOS driver
opts = { caps: { platformName: :ios, app: '/path/to/MyiOS.app' } }
Appium::Driver.new(opts).start_driver

# Start Android driver
opts = { caps: { platformName: :android, app: '/path/to/my.apk' } }
Appium::Driver.new(opts).start_driver
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Object] opts - A hash containing various options.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Driver] 

--

##### [driver_attributes](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L334) 

> def driver_attributes

Returns a hash of the driver attributes

--

##### [device_is_android?](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L354) 

> def device_is_android?



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Boolean] 

--

##### [appium_server_version](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L370) 

> def appium_server_version

Returns the server's version info

```ruby
{
    "build" => {
        "version" => "0.18.1",
        "revision" => "d242ebcfd92046a974347ccc3a28f0e898595198"
    }
}
```

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] 

--

##### [absolute_app_path](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L382) 

> def self.absolute_app_path opts

Converts app_path to an absolute path.

opts is the full options hash (caps and appium_lib). If server_url is set
then the app path is used as is.

if app isn't set then an error is raised.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] APP_PATH as an absolute path

--

##### [server_url](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L415) 

> def server_url

Get the server url

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] the server url

--

##### [restart](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L426) 

> def restart

Restarts the driver

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Driver] the driver

--

##### [driver](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L433) 

> def driver

Returns the driver

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Driver] the driver

--

##### [screenshot](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L443) 

> def screenshot png_save_path

Takes a png screenshot and saves to the target path.

Example: screenshot '/tmp/hi.png'

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] png_save_path - the full path to save the png

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[nil] 

--

##### [driver_quit](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L450) 

> def driver_quit

Quits the driver

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [start_driver](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L458) 

> def start_driver

Creates a new global driver and quits the old one if it exists.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Selenium::WebDriver] the new global driver

--

##### [no_wait](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L485) 

> def no_wait

Set implicit wait and default_wait to zero.

--

##### [set_wait](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L504) 

> def set_wait timeout=nil

Set implicit wait and default_wait to timeout, defaults to 30.
if set_wait is called without a param then the second to last
wait will be used.

```ruby`
set_wait 2
set_wait 3
set_wait # 2

````

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Integer] timeout - the timeout in seconds

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [exists](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L538) 

> def exists pre_check=0, post_check=@default_wait, &search_block

Returns existence of element.

Example:

exists { button('sign in') } ? puts('true') : puts('false')

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Integer] pre_check - the amount in seconds to set the
wait to before checking existance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Integer] post_check - the amount in seconds to set the
wait to after checking existance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Block] search_block - the block to call

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Boolean] 

--

##### [execute_script](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L562) 

> def execute_script script, *args

The same as @driver.execute_script

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] script - the script to execute

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[*args] args - the args to pass to the script

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Object] 

--

##### [find_elements](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L570) 

> def find_elements *args

Calls @driver.find_elements

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[*args] args - the args to use

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Element>] Array is empty when no elements are found.

--

##### [find_element](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L578) 

> def find_element *args

Calls @driver.find_elements

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[*args] args - the args to use

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [x](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/driver.rb#L585) 

> def x

Quit the driver and Pry.
quit and exit are reserved by Pry.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [NoArgMethods](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L7) 

> NoArgMethods = {



--

##### [app_strings](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L22) 

> def app_strings

Return the hash of all localization strings.
```ruby
app_strings #=> "TransitionsTitle"=>"Transitions", "WebTitle"=>"Web"
```

--

##### [background_app](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L28) 

> def background_app

Backgrounds the app for a set number of seconds.
This is a blocking application

--

##### [current_activity](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L33) 

> def current_activity



--

##### [launch](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L35) 

> def launch

Start the simulator and applicaton configured with desired capabilities

--

##### [reset](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L38) 

> def reset

Reset the device, relaunching the application.

--

##### [shake](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L41) 

> def shake

Cause the device to shake

--

##### [toggle_flight_mode](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L44) 

> def toggle_flight_mode

toggle flight mode on or off

--

##### [hide_keyboard](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L47) 

> def hide_keyboard

Hide the onscreen keyboard

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] close_key - the name of the key which closes the keyboard.
Defaults to 'Done'.

--

##### [press_keycode](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L56) 

> def press_keycode

Press keycode on the device.
http://developer.android.com/reference/android/view/KeyEvent.html

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[integer] key - The key to press.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] metastate - The state the metakeys should be in when pressing the key.

--

##### [long_press_keycode](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L62) 

> def long_press_keycode

Long press keycode on the device.
http://developer.android.com/reference/android/view/KeyEvent.html

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[integer] key - The key to long press.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] metastate - The state the metakeys should be in when long pressing the key.

--

##### [push_file](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L68) 

> def push_file

Place a file in a specific location on the device.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] path - The absolute path on the device to store data at.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] data - Raw file data to be sent to the device.

--

##### [pull_file](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L73) 

> def pull_file

Retrieve a file from the device.  This can retrieve an absolute path or
a path relative to the installed app (iOS only).
```ruby
pull_file '/local/data/some/path' #=> Get the file at that path
pull_file 'Shenanigans.app/some/file' #=> Get 'some/file' from the install location of Shenanigans.app
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] path - Either an absolute path OR, for iOS devices, a path relative to the app, as described.

--

##### [pull_folder](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L83) 

> def pull_folder

Retrieve a folder from the device.
```ruby
pull_folder '/data/local/tmp' #=> Get the folder at that path
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] path - absolute path to the folder

--

##### [extend_search_contexts](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L274) 

> def extend_search_contexts



--

##### [accessiblity_id_find](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L274) 

> def accessiblity_id_find

find_element/s with their accessibility_id

```ruby
 find_elements :accessibility_id, 'Animation'
```

--

##### [add_touch_actions](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L280) 

> def add_touch_actions



--

##### [set_context](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L304) 

> def set_context

Change the context to the given context.
```ruby
set_context "NATIVE_APP"
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] The - context to change to

--

##### [current_context](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L312) 

> def current_context



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] The context currently being used.

--

##### [available_contexts](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L315) 

> def available_contexts



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<String>] All usable contexts, as an array of strings.

--

##### [within_context](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L325) 

> def within_context(context)

Perform a block within the given context, then switch back to the starting context.
```ruby
within_context('NATIVE_APP') do
  find_element [:tag, "button"]
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] context - The context to switch to for the duration of the block.

--

##### [switch_to_default_context](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/device.rb#L333) 

> def switch_to_default_context

Change to the default context.  This is equivalent to `set_context nil`.

--

##### [pinch](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/multi_touch.rb#L30) 

> def pinch(percentage=25, auto_perform=true)

Convenience method for pinching the screen.
Places two fingers at the edges of the screen and brings them together.
```ruby
action = pinch 75 #=> Pinch the screen from the top right and bottom left corners
action.perform    #=> to 25% of its size.
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[int] percentage - The percent size by which to shrink the screen when pinched.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[boolean] auto_perform - Whether to perform the action immediately (default true)

--

##### [zoom](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/multi_touch.rb#L58) 

> def zoom(percentage=200, auto_perform=true)

Convenience method for zooming the screen.
Places two fingers at the edges of the screen and brings them together.
```ruby
action = zoom 200 #=> Zoom in the screen from the center until it doubles in size.
action.perform
```

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[int] percentage - The percent size by which to shrink the screen when pinched.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[boolean] auto_perform - Whether to perform the action immediately (default true)

--

##### [initialize](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/multi_touch.rb#L79) 

> def initialize

Create a new multi-action

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[MultiTouch] a new instance of MultiTouch

--

##### [add](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/multi_touch.rb#L85) 

> def add(chain)

Add a touch_action to be performed

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TouchAction] chain - The action to add to the chain

--

##### [perform](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/multi_touch.rb#L90) 

> def perform

Ask Appium to perform the actions

--

##### [ACTIONS](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L12) 

> ACTIONS         = [:move_to, :long_press, :press, :release, :tap, :wait, :perform]



--

##### [COMPLEX_ACTIONS](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L13) 

> COMPLEX_ACTIONS = [:swipe]



--

##### [actions](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L27) 

> def actions

Returns the value of attribute actions

--

##### [initialize](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L29) 

> def initialize



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TouchAction] a new instance of TouchAction

--

##### [move_to](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L37) 

> def move_to(opts)

Move to the given co-ordinates.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - a customizable set of options

--

##### [long_press](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L47) 

> def long_press(opts)

Press down for a specific duration.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] element - a customizable set of options

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] x - a customizable set of options

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] y - a customizable set of options

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] duration - a customizable set of options

--

##### [press](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L59) 

> def press(opts)

Press a finger onto the screen.  Finger will stay down until you call
`release`.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - a customizable set of options

--

##### [release](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L70) 

> def release(opts=nil)

Remove a finger from the screen.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - a customizable set of options

--

##### [tap](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L81) 

> def tap(opts)

Touch a point on the screen

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - a customizable set of options

--

##### [wait](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L90) 

> def wait(milliseconds)

Pause for a number of milliseconds before the next action

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[integer] milliseconds - Number of milliseconds to pause for

--

##### [swipe](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L104) 

> def swipe(opts)

Convenience method to peform a swipe.

Note that iOS 7 simulators have broken swipe.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - a customizable set of options

--

##### [perform](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L119) 

> def perform

Ask the driver to perform all actions in this action chain.

--

##### [cancel](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L125) 

> def cancel

Does nothing, currently.

--

##### [chain_method](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L133) 

> def chain_method(method, args=nil)



--

##### [args_with_ele_ref](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/device/touch_actions.rb#L142) 

> def args_with_ele_ref(args)



--

##### [_generic_wait](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/wait.rb#L10) 

> def _generic_wait opts={}, &block

Wait code from the selenium Ruby gem
https://github.com/SeleniumHQ/selenium/blob/cf501dda3f0ed12233de51ce8170c0e8090f0c20/rb/lib/selenium/webdriver/common/wait.rb

--

##### [_process_wait_opts](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/wait.rb#L55) 

> def _process_wait_opts opts

process opts before calling _generic_wait

--

##### [wait_true](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/wait.rb#L76) 

> def wait_true opts={}, &block

Check every interval seconds to see if block.call returns a truthy value.
Note this isn't a strict boolean true, any truthy value is accepted.
false and nil are considered failures.
Give up after timeout seconds.

Wait code from the selenium Ruby gem
https://github.com/SeleniumHQ/selenium/blob/cf501dda3f0ed12233de51ce8170c0e8090f0c20/rb/lib/selenium/webdriver/common/wait.rb

If only a number is provided then it's treated as the timeout value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - Options

--

##### [wait](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/wait.rb#L94) 

> def wait opts={}, &block

Check every interval seconds to see if block.call doesn't raise an exception.
Give up after timeout seconds.

Wait code from the selenium Ruby gem
https://github.com/SeleniumHQ/selenium/blob/cf501dda3f0ed12233de51ce8170c0e8090f0c20/rb/lib/selenium/webdriver/common/wait.rb

If only a number is provided then it's treated as the timeout value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] opts - Options

--

##### [ignore](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L22) 

> def ignore &block

Return block.call and ignore any exceptions.

--

##### [back](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L31) 

> def back

Navigate back.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [session_id](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L36) 

> def session_id

For Sauce Labs reporting. Returns the current session id.

--

##### [xpath](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L44) 

> def xpath xpath_str

Returns the first element that matches the provided xpath.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] xpath_str - the XPath string

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [xpaths](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L52) 

> def xpaths xpath_str

Returns all elements that match the provided xpath.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] xpath_str - the XPath string

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Element>] 

--

##### [source](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L58) 

> def source

Prints xml of the current page

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [get_source](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L76) 

> def get_source

Returns XML string for the current page
Same as driver.page_source

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] 

--

##### [result](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L83) 

> def result

Returns the value of attribute result

--

##### [initialize](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L85) 

> def initialize



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[CountElements] a new instance of CountElements

--

##### [reset](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L89) 

> def reset



--

##### [start_element](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L94) 

> def start_element name, attrs = []

http://nokogiri.org/Nokogiri/XML/SAX/Document.html

--

##### [formatted_result](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L100) 

> def formatted_result



--

##### [get_page_class](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L111) 

> def get_page_class

Returns a string of class counts of visible elements.

--

##### [page_class](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L122) 

> def page_class

Count all classes on screen and print to stdout.
Useful for appium_console.

--

##### [px_to_window_rel](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L132) 

> def px_to_window_rel opts={}

Converts pixel values to window relative values

```ruby
px_to_window_rel x: 50, y: 150
```

--

##### [xml_keys](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L149) 

> def xml_keys target

Search strings.xml's values for target.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] target - the target to search for in strings.xml values

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array] 

--

##### [xml_values](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L157) 

> def xml_values target

Search strings.xml's keys for target.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] target - the target to search for in strings.xml keys

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array] 

--

##### [resolve_id](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L165) 

> def resolve_id id

Resolve id in strings.xml and return the value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] id - the id to resolve

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] 

--

##### [filter](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L171) 

> def filter



--

##### [filter=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L176) 

> def filter= value

convert to string to support symbols

--

##### [initialize](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L182) 

> def initialize



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[HTMLElements] a new instance of HTMLElements

--

##### [reset](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L187) 

> def reset



--

##### [result](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L193) 

> def result



--

##### [start_element](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L207) 

> def start_element name, attrs = []



--

##### [end_element](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L217) 

> def end_element name



--

##### [characters](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/helper.rb#L223) 

> def characters(chars)



--

##### [window_size](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/element/window.rb#L5) 

> def window_size

Get the window's size

--

##### [result](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L6) android

> def result

Returns the value of attribute result

--

##### [keys](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L6) android

> def keys

Returns the value of attribute keys

--

##### [instance](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L6) android

> def instance

Returns the value of attribute instance

--

##### [filter](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L8) android

> def filter



--

##### [filter=](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L13) android

> def filter= value

convert to string to support symbols

--

##### [initialize](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L19) android

> def initialize



__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[AndroidElements] a new instance of AndroidElements

--

##### [reset](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L25) android

> def reset



--

##### [start_element](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L32) android

> def start_element name, attrs = []

http://nokogiri.org/Nokogiri/XML/SAX/Document.html

--

##### [get_android_inspect](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L92) android

> def get_android_inspect class_name=false

Android only.
Returns a string containing interesting elements.
The text, content description, and id are returned.
if false (default) then all classes will be inspected

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the class name to filter on.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] 

--

##### [page](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L113) android

> def page opts={}

Intended for use with console.
Inspects and prints the current page.
Will return XHTML for Web contexts because of a quirk with Nokogiri.
if nil (default) then all classes will be inspected

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hash] class - a customizable set of options

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [current_app](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L124) android

> def current_app

example line:
"mFocusedApp=AppWindowToken{b1420058 token=Token{b128add0 ActivityRecord{b1264d10 u0 com.example.android.apis/.ApiDemos t23}}}"

--

##### [id](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L148) android

> def id id

Find the first matching element by id

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] id - the id to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [ids](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L156) android

> def ids id

Find all matching elements by id

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] id - the id to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [ele_index](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L165) android

> def ele_index class_name, index

Find the element of type class_name at matching index.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the class name to find

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Integer] index - the index

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] the found element of type class_name

--

##### [first_ele](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L183) android

> def first_ele class_name

Find the first element that matches class_name

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the tag to match

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [last_ele](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L190) android

> def last_ele class_name

Find the last element that matches class_name

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the tag to match

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [tag](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L198) android

> def tag class_name

Find the first element of type class_name

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the class_name to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [tags](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L206) android

> def tags class_name

Find all elements of type class_name

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the class_name to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [complex_find_contains](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L238) android

> def complex_find_contains element, value

Find the first element that contains value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] element - the class name for the element

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [complex_finds_contains](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L246) android

> def complex_finds_contains element, value

Find all elements containing value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] element - the class name for the element

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Element>] 

--

##### [complex_find_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L275) android

> def complex_find_exact class_name, value

Find the first element exactly matching value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the class name for the element

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [complex_finds_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/helper.rb#L283) android

> def complex_finds_exact class_name, value

Find all elements exactly matching value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] class_name - the class name for the element

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [TextView](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L4) android

> TextView = 'android.widget.TextView'



--

##### [text](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L10) android

> def text value

Find the first TextView that contains value or by index.
If int then the TextView at that index is returned.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String, Integer] value - the value to find.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TextView] 

--

##### [texts](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L19) android

> def texts value=false

Find all TextViews containing value.
If value is omitted, all texts are returned.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<TextView>] 

--

##### [first_text](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L26) android

> def first_text

Find the first TextView.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TextView] 

--

##### [last_text](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L32) android

> def last_text

Find the last TextView.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TextView] 

--

##### [text_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L39) android

> def text_exact value

Find the first TextView that exactly matches value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to match exactly

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TextView] 

--

##### [texts_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/text.rb#L46) android

> def texts_exact value

Find all TextViews that exactly match value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to match exactly

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<TextView>] 

--

##### [_nodeset_to_uiselector](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/client_xpath.rb#L5) android

> def _nodeset_to_uiselector opts={}



--

##### [_client_xpath](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/client_xpath.rb#L20) android

> def _client_xpath opts={}



--

##### [client_xpath](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/client_xpath.rb#L36) android

> def client_xpath xpath



--

##### [client_xpaths](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/client_xpath.rb#L40) android

> def client_xpaths xpath



--

##### [alert_click](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/alert.rb#L6) android

> def alert_click value

Click the first alert button that contains value or by index.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Integer, String] value - either an integer index of the button or the button's name

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [alert_accept](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/alert.rb#L13) android

> def alert_accept

Accept the alert.
The last button is considered "accept."

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [alert_accept_text](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/alert.rb#L20) android

> def alert_accept_text

Get the text of the alert's accept button.
The last button is considered "accept."

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] 

--

##### [alert_dismiss](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/alert.rb#L27) android

> def alert_dismiss

Dismiss the alert.
The first button is considered "dismiss."

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[void] 

--

##### [alert_dismiss_text](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/alert.rb#L34) android

> def alert_dismiss_text

Get the text of the alert's dismiss button.
The first button is considered "dismiss."

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] 

--

##### [uiautomator_find](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/mobile_methods.rb#L10) android

> def uiautomator_find

find_element/s can be used with a [UISelector](http://developer.android.com/tools/help/uiautomator/UiSelector.html).

```ruby
 find_elements :uiautomator, 'new UiSelector().clickable(true)'
```

--

##### [Button](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L4) android

> Button      = 'android.widget.Button'



--

##### [ImageButton](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L5) android

> ImageButton = 'android.widget.ImageButton'



--

##### [button](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L43) android

> def button value

Find the first button that contains value or by index.
If int then the button at that index is returned.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String, Integer] value - the value to exactly match.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Button] 

--

##### [buttons](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L60) android

> def buttons value=false

Find all buttons containing value.
If value is omitted, all buttons are returned.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Button>] 

--

##### [first_button](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L67) android

> def first_button

Find the first button.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Button] 

--

##### [last_button](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L73) android

> def last_button

Find the last button.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Button] 

--

##### [button_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L89) android

> def button_exact value

Find the first button that exactly matches value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to match exactly

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Button] 

--

##### [buttons_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/button.rb#L96) android

> def buttons_exact value

Find all buttons that exactly match value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to match exactly

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Button>] 

--

##### [find](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/generic.rb#L7) android

> def find value

Find the first element containing value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [finds](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/generic.rb#L14) android

> def finds value

Find all elements containing value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Element>] 

--

##### [find_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/generic.rb#L21) android

> def find_exact value

Find the first element exactly matching value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] 

--

##### [finds_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/generic.rb#L28) android

> def finds_exact value

Find all elements exactly matching value

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<Element>] 

--

##### [scroll_to](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/generic.rb#L40) android

> def scroll_to text

Scroll to the first element containing target text or description.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] text - the text to search for in the text value and content description

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] the element scrolled to

--

##### [scroll_to_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/generic.rb#L52) android

> def scroll_to_exact text

Scroll to the first element with the exact target text or description.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] text - the text to search for in the text value and content description

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Element] the element scrolled to

--

##### [EditText](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L3) android

> EditText = 'android.widget.EditText'



--

##### [textfield](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L9) android

> def textfield value

Find the first EditText that contains value or by index.
If int then the EditText at that index is returned.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String, Integer] value - the text to match exactly.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[EditText] 

--

##### [textfields](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L18) android

> def textfields value=false

Find all EditTexts containing value.
If value is omitted, all EditTexts are returned.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to search for

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<EditText>] 

--

##### [first_textfield](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L25) android

> def first_textfield

Find the first EditText.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[EditText] 

--

##### [last_textfield](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L31) android

> def last_textfield

Find the last EditText.

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[EditText] 

--

##### [textfield_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L38) android

> def textfield_exact value

Find the first EditText that exactly matches value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to match exactly

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[EditText] 

--

##### [textfields_exact](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/android/element/textfield.rb#L45) android

> def textfields_exact value

Find all EditTexts that exactly match value.

__Parameters:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[String] value - the value to match exactly

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Array<EditText>] 

--

##### [value](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/patch.rb#L10) 

> def value

Returns the value attribute

Fixes NoMethodError: undefined method `value' for Selenium::WebDriver::Element

--

##### [name](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/patch.rb#L17) 

> def name

Returns the name attribute

Fixes NoMethodError: undefined method `name' for Selenium::WebDriver::Element

--

##### [location_rel](https://github.com/appium/ruby_lib/blob/a13158fb926212d84f26120c3bc5355c8cd34baf/lib/appium_lib/common/patch.rb#L29) 

> def location_rel

For use with mobile tap.

```ruby
execute_script 'mobile: tap', :x => 0.0, :y => 0.98
```

https://github.com/appium/appium/wiki/Automating-mobile-gestures

__Returns:__

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[OpenStruct] the relative x, y in a struct. ex: { x: 0.50, y: 0.20 }

--

