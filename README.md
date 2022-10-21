# icon.community – The Official ICON Community Website

The icon.community website is the main hub to direct members of the ICON ecosystem to available resources. This site includes blogs, links to other media, and general information about the ICON community!

This repository contains the code and assets for the [icon.community](https://icon.community) site. To preview the site in a local environment, you'll need to install the Hugo static site generator.

## How to Install Hugo

Hugo supports multiple platforms including macOS, Windows, and Linux.

### macOS and Linux

For macOS and Linux users, we recommend using Homebrew to install Hugo.

```
brew install hugo
```

### Windows

For Windows users, we recommend using Chocolatey to install Hugo.

```
choco install hugo -confirm
```

## How to Preview the Site Locally

After installing Hugo, navigate to the project directory and install the npm dependencies with the command below.

```
npm install
```

Once the dependencies have been installed, run the command below to start a local Hugo server.

```
hugo server
```

Whenever you make a change to the site code or content, Hugo will automatically rebuild the site.

# Shortcodes

The icon.community site is equipped with a variety of shortcodes that can be used with content files.

* [discord](#discord)
* [table](#table)

## discord

This shortcode inserts an anchor element with the href attribute set to an invite link for the ICON Discord.

```
{{< discord >}}

// Output

<a href="https://discord.com/invite/7a75Hf3cFm">Discord</a>
```

```
{{< discord linkText="Join the ICON Discord!" >}}

// Output

<a href="https://discord.com/invite/7a75Hf3cFm">Join the ICON Discord!</a>
```

## table

This shortcode converts a Markdown table to an HTML table.

```
{{< table >}}
| Header A | Header B |
|----------|----------|
| Lorem    | Ipsum    |
| Foo      | Bar      |
{{< /table >}}

// Output

<div class="overflow-x-auto">
    <table>
        <thead>
            <tr>
                <th>Header A</th>
                <th>Header B</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Lorem</td>
                <td>Ipsum</td>
            </tr>
            <tr>
                <td>Foo</td>
                <td>Bar</td>
            </tr>
        </tbody>
    </table>
</div>

```