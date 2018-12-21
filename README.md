# WP Ajaxer
Simple Lightweight Ajax Handler For WP Theme/Plugin Developers


## Installation
The preferred way to install this extension is through [Composer](http://getcomposer.org/download/).

To install **WP_Ajaxer library**, simply:

    $ composer require Varunsridharan/WP_Ajaxer

The previous command will only install the necessary files, if you prefer to **download the entire source code** you can use:

    $ composer require Varunsridharan/WP_Ajaxer --prefer-source

You can also **clone the complete repository** with Git:

    $ git clone https://github.com/varunsridharan/wp-ajaxer.git

Or **install it manually**:

[Download WP_Ajaxer.php](https://raw.githubusercontent.com/varunsridharan/wp-ajaxer/master/class-ajaxer.php):

    $ wget https://raw.githubusercontent.com/varunsridharan/wp-ajaxer/master/class-ajaxer.php



## Sample Usage
```php

class BoilerPlate_Ajax extends Varunsridharan\WordPress\Ajaxer {
	/**
	 * Ajax Action Prefix
	 *
	 * @example for wordpress_show_popup wordpress is the prefix
	 *
	 * @var string
	 */
	protected $action_prefix = 'bp';

	/**
	 * Ajax Action Surfix
	 *
	 * @example for wordpress_show_popup_data data is the surfix
	 *
	 * @var string
	 */
	protected $action_surfix = '';

	/**
	 * Action Name
	 * provide value if all ajax requests runs in a single action key.
	 *
	 * @var string
	 */
	protected $action = 'bp-plugin';

	/**
	 * Array of ajax actions
	 *
	 * @example array('ajax_action_1' => true,'ajax_action_2' => false)
	 *          if value set to true then it runs for both loggedout / logged in users
	 *          if value set to false then it runs only for the logged in user
	 *
	 * @var array
	 */
	protected $actions = array(
		'action1'   => false,
		'action-12' => false,
	);

	/**
	 * Set to true if plugin's ajax runs in a single action
	 *
	 * @example Single Ajax Action
	 *          admin-ajax.php?action=plugin-slug&plugin-slug-action=ajax-action&param1=value1&param2=value=2
	 *          Multiple Ajax Actions
	 *          admin-ajax.php?action=plugin-slug-ajax-action1&param1=value1=param2=value2
	 *
	 * @var bool
	 */
	protected $is_single = true;

	/**
	 * Provide a action key if $this->is_single is set to true
	 *
	 * @var string
	 */
	protected $single_ajax_key = '';

	public function __construct( ) {
		parent::__construct();
	}

	public function action1() {
		///do some action here
	}
}
```


---
## Sponsored By
[![DigitalOcean](https://vsp.ams3.cdn.digitaloceanspaces.com/cdn/DO_Logo_Horizontal_Blue.png)](https://s.svarun.in/Ef)

