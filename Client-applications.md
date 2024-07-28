# Client Applications and the Core Package

## Applications

There are two client applications.

### bisonw

Most users will want to use the **browser-based GUI** for Bison Wallet.  It
offers a familiar wallet and exchange experience in your browser.  The market
view allows you to see the market's order book in sorted lists or as a depth
chart.  You can place an order and monitor its status in the same market view.

The GUI app is managed by the **bisonw** utility in `dcrdex/client/cmd/bisonw`.
This utility is really just a one-client web server that you run and connect to
on the same machine. 

See the [Bison Wallet Installation and Configuration](https://github.com/decred/dcrdex/wiki/Client-Installation-and-Configuration)
page for a detailed walkthrough of the initial setup.

### bwctl

The **bwctl** utility enables trading via CLI. Commands are parsed and
issued to **Core** for execution. **bwctl** also requires **bisonw**.

## Core client Go language package

For developers, the `dcrdex/client/core` Go language package provides the
`Core` client type, which offers an intuitive programmer interface, with
methods for creating wallets, registering DEX accounts, viewing markets, and
performing trades.
