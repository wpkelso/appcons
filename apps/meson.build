fs = import('fs')
icon_sizes = ['16', '24', '32', '48', '64', '128']

icon_links = [
    # The first argument is the original icon name,
    # the second is the link.
    # `alt` files do not get symlinked,
    # they should be changed in the relevant `desktop` file

    ['alacritty', 'com.alacritty.Alacritty'],
    ['alacritty', 'Alacritty'],

    ['slack', 'com.slack.Slack'],

    ['obsidian', 'md.obsidian.Obsidian'],

    ['zotero', 'org.zotero.Zotero']
]

foreach link : icon_links
    foreach size : icon_sizes
        # only symlink to files that actually exist
        if fs.is_file(size / link[0] + '.svg')
            install_symlink(
                link[1] + '.svg',
                install_dir: icon_dir / 'apps' / size,
                pointing_to: link[0] + '.svg',
            )
        endif
    endforeach
endforeach
