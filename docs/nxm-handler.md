# Send download to specific Mod Manager

!!! info "The website provides a 'Mod Manager' download button that sends it to the user's mod manager."

- Status: Unknown/Shortlisted 

<figure markdown="span">
  ![images](./images/mod-manager-download.webp)
  <figcaption>'Mod Manager' download button, as seen today.</figcaption>
</figure>

Pressing this button opens a URL that starts with `nxm://`; and it is sent to the last application
on the user's computer that said `'I can handle nxm://'`.

## Problems

### Vortex Vendor Lock-In

!!! warning "*One click download is ONLY allowed for games supported by Vortex Mod Manager*"

    The current site policy is to now allow the 'Mod Manager' download
    button to be shown unless a game is supported by Vortex Mod Manager.(1)
    { .annotate }

    1. Excludes a single digit number of 'legacy games' from before the policy was introduced.

This is stated to be in order to 'avoid confusion', but it goes against our core ethos of
*making modding easy*.

Without a *'mod manager download'* button, users would have to explicitly read
the *mod description* in order to learn how to install a mod.

In a world where attention spans are short, people expect things to *'just work'* and for many people
are ***new to modding*** this creates a barrier to entry. Especially affected are smaller, less popular
games which have the potential to become big in the future.

!!! info "In the past this has prevented myself from integrating with the Nexus Mods website."

If someone creates a piece of software that supports modding for a game, they should be able to get
a working *'Mod Manager'* download button for it, with the appropriate branding.

The current limitation often leads to the creation of 'low effort' plugins to Vortex.
Some Vortex plugins just end up setting up an entirely different modding tool/mod manager entirely,
delegating only download requests to it to get the coveted 'Download Button'.

Other times, Vortex plugins are made as barebones as possible and are never updated again.
They become broken, and unsupported, *making easy modding hard*.

!!! warning "Vortex is only available on Windows"

    Users on other operating systems (e.g. Linux, macOS) ***cannot even natively run Vortex***;
    effectively locking them out of the *'Mod Manager Download'* button without massive, difficult
    hacks.

!!! info "This also creates issues for our very own `Nexus Mods App`"

### Sending Downloads to the Wrong Mod Manager

!!! tip "Clicking the button sends the download to the last mod manager that registered for `nxm://` links."

    This may not be the mod manager that the user wants to use.

For example suppose a user has Vortex (or Nexus Mods App) and different mod manager installed.

One of the games they are modding is not supported by Vortex, but is supported by another manager.

Currently, if the user clicks the 'Mod Manager' download button, it will send the download to Vortex
if Vortex was the last opened program, as it would have registered itself as the handler for `nxm://`
links.

!!! info "Some 'proxy' tools already exist."

    Namely:

    - [nxmproxy](https://github.com/TanninOne/nxmproxy): Which is a commandline only tool (requires good computer literacy).
    - [nxmhandler](https://github.com/ModOrganizer2/modorganizer-nxmhandler): Part of Mod Organizer 2.

    These tools however only work on Windows; and have limitations, such as only supporting a fixed
    set of games in the case of `nxmhandler`.

On many mod pages for smaller games, there might only be one supported mod manager.

## What I Want

