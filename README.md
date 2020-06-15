# LND-For-WP  - v0.1.2
## A WordPress plugin for managing &amp; using your LND node.

### Description
LND For WP is a WordPress plugin that allows you to manage and use your LND node, right from your WordPress administration panel. It provides a fully functional wallet interface, allowing you to send and recieve funds across the Lightning Network with ease. The user interface is responsive and will adapt to fit any web enabled desktop, tablet or mobile device. You can search the Lightning Network graph, manage peer connections and open & close channels with ease.
The plugin has QR support, enabling basic encoding & decoding of QR codes.
LND For WP also adds a number of WordPress 'shortcodes', allowing you to embed LND functionality directly in your website pages and posts. New Shortcodes will be added with future versions, as needs & use cases arise.

![Plugin Preview](/lnd-for-wp-preview.png?raw=true "LND For WP Preview")

### Installation

LND For WP can be installed directly from WordPress. Simply navigate to the 'Plugins -> Add New' page and search for 'LND For WP'. You can also view LND For WP on the [WordPress.org Plugin Directory](https://wordpress.org/plugins/lnd-for-wp/)

To install the plugin manually using source code from this repository:

1. Download the latest plugin release from this repository.
2. Browse to the 'Plugins -> Add New' page of your WordPress admin panel.
3. Click the 'Upload Plugin' button, select 'Browse' and choose the release .zip that you downloaded in step 1.
4. Press 'Install Now'.
5. On the next screen, press the 'Activate' button to turn on the plugin.
6. You're done. You should now see the 'LND For WP' link on your WP admin navigation menu.

### Shortcodes

1. Paywall: [lnd paywall amount=1 memo="https://dev.adelberg-online.de/?p=394"]Your content[/lnd]
2. Donation: [lnd lightning_invoice ajax="true" amount=1 memo="https://dev.adelberg-online.de/?p=394"]
3. Onchain address: [lnd on_chain_address generate_new="true"]
4. Current version: [lnd current_version]

### Frequently Asked Questions

#### 1. What is LND?
  LND stands for 'Lightning Network Daemon'. It's a software implementation of the 'Lightning Network', which is an open protocol layer that leverages the power of blockchains and smart contracts to make cheap, fast, private transactions available to anyone around the world. To learn more, visit [Lightning Labs - Technology Overview](https://lightning.engineering/technology.html).

#### 2. Where can I download the latest version of LND?
   https://github.com/lightningnetwork/lnd/releases

#### 3. LND is up and running. Where are my macaroons?
  Your macaroon files are generated automatically by LND when it is started. Assuming you're running Bitcoin on mainnet, you would find them inside the data/chain/bitcoin/mainnet directory of your LND dir. By default, the LND dir is located at:
`~/.lnd` on Linux
`/Users/[username]/Library/Application Support/Lnd/` on Mac OSX
or `$APPDATA/Local/Lnd` on Windows.


### Contributing
Contributions in the form of issues, feedback & pull requests are welcome.<br />
