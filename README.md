# tumblr-likes
[![Crates.io](https://img.shields.io/crates/v/tumblr-likes.svg)](https://crates.io/crates/tumblr-likes)

### A command-line program for downloading liked posts from Tumblr.

## Installation

Download the [latest release for your platform](https://github.com/subnomo/tumblr-likes/releases).

Or, using cargo:

```
$ cargo install tumblr-likes
```

## Configuration

In order to download liked posts, you will need an API key.

1. [Register an application with the Tumblr API](https://www.tumblr.com/oauth/apps). The name and other options don't matter.
2. Click "Expore API" under the application you just created
3. Click "Allow"
4. In the upper right, click "Show Keys"
5. Copy the API key shown

## Usage

On the command line:

```
$ tumblr-likes -a <api_key> -b <blog>
```

If you don't want to provide the API key every time, you can save it into an environmental variable `$TUMBLR_API_KEY` instead.

By default, liked posts will be downloaded into a `downloads` folder in the current directory. You can use `-d` to set a custom output directory.

---

This is very similar to a [Node.js package I created](https://github.com/subnomo/tumblr-like-dl) a few years ago. I noticed it was getting an surge of installs recently, most likely because [Tumblr decided to ban adult content](https://www.theverge.com/2018/12/3/18123752/tumblr-adult-content-porn-ban-date-explicit-changes-why-safe-mode). That package doesn't work anymore though, so I rewrote it in Rust. If you were trying to use that package, sorry.
