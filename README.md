# 📤 PairDrop Rooms

## Self-Hosted File Sharing

[PairDrop Rooms](https://pairdrop.org) is a **self-contained, open-source PHP script** for sharing files. Designed to be simple to use via a web browser, PairDrop Rooms offers maximum **privacy** as a self-hosted service.

The script requires no database, complex dependencies, or elaborate configuration. A single `index.php` file handles everything, from creating *private rooms* to managing uploads and downloads.

#### Table of Contents

- [Why choose PairDrop Rooms?](#why-choose-pairdrop-rooms)
- [What is different here?](#what-is-different-here)
- [Quick Installation Guide](#quick-installation-guide)
- [Requirements](#requirements)
- [Live Demo](#live-demo)

## Why choose PairDrop Rooms?

✅ **Maximum Privacy**  
Complete control over your data and files with no third-parties. The script and files are on *your* server.

🚀 **Fast and Lightweight**  
Purely simple PHP for minimal execution time and low server load. No frameworks, **no database**.
   
🔑 **Private Code-Protected Rooms**  
Share files in unique, private rooms. Only those with the room code can access and view the files.

⚫ **Modern, Mobile Friendly Design**  
Features a modern and clean design that is **mobile-friendly** featuring both Light Mode and Dark Mode themes.

## What is different here?

This is a fork of [PairDrop.org](https://pairdrop.org/) with some additional changes / features. The original author of PairDrop.org, whose name is unknown, calls the software Open-Source in several locations, but left no contact information.

Please reach out, let's collaborate! My email address is on my website. \<[https://timi.me](https://timi.me)\> ✌️

---

🔐 **Private Mode Setting**  
When enabled, a room code directory must already exist on the server for the visitor to be allowed in. The script will no longer automatically create room directories, they must already exist (i.e. *you* create them).

This functionality offers a more private space to quickly and easily share files between colleagues.

Change this setting to `false`:

```php
define('ALLOW_CREATE_ROOMS', true);
```

🐞 **Improved Error Handling**  
This fork of PairDrop Rooms handles upload errors a little better. It's still bad, a simple JavaScript `alert();`, but it used to just silently fail.

## Quick Installation Guide

Assuming you know how to use a PHP script, installation and use is super simple.

1. Adjust settings in the `CONFIGURATION` section of `index.php`
2. Create a directory for PairDrop Rooms on your server (e.g. `/drop/`)  
<small style="color:#f00">Ensure PHP has write permissions for this directory</small>  
3. Upload the configured `index.php` into the `/drop/` folder
4. Done!

Open your browser and navigate to the URL where you created the directory in Step 2. Enter a room code and start sharing files!

## Requirements

- PHP 7.4+
- Write permissions

## Live Demo

Until I hear from the original author, navigate to the [PairDrop.org](https://pairdrop.org) website to find the live demo links. Keep in mind that their live demo does not [feature this fork's changes](#what-is-different-here).
