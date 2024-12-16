icon_sizes = ['16', '24', '32', '48', '64', '128']

icon_links = [
    # The first argument is the original icon name,
    # the second is the link.
    # `alt` files to not get symlinked,
    # they should be changed in the relevant `desktop`` file

    ['alacritty', 'com.alacritty.Alacritty'],
    ['alacritty', 'Alacritty'],

    ['zen-browser', 'io.github.zen_browser.zen'],

    ['slack', 'com.slack.Slack'],

    ['bitwarden', 'com.bitwarden.desktop'],

    ['obsidian', 'md.obsidian.Obsidian'],

    ['inkscape', 'org.inkscape.Inkscape'],

    ['zotero', 'org.zotero.Zotero']
]

foreach link : icon_links
    foreach size : icon_sizes
        install_symlink(
            link[1] + '.svg',
            install_dir: icon_dir / 'apps' / size,
            pointing_to: link[0] + '.svg',
        )
    endforeach
endforeach
