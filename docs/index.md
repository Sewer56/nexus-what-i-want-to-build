# What does Seweryn want to build?

!!! question "What would you build if you had a magic wand?"

    *Is what the Chosen Ones said.*

Having had a lot of thoughts for a long time, and never the proper time to compile them, I might just
take the time to list some of them here. 😉

This is my own wishlist, some of the items here are things I have already started working on
(alone, in my own time) and some are just ideas for the site itself
that I think would be essential to have.

Having been a mod tool author for nearly a decade, the 

## About Me

Hi, I'm Seweryn (aka Sewer56), a `"full-stack modder"` and open source library author working as one of the guys at the App Team.
I'm probably one of the few people that can say I've worked on every aspect of modding: Libraries,
Mod Loaders, Mod Managers, Modding Tools, Adding Online Multiplayer to Single Player games; you name it;
sometimes I lose track of what I've done myself 😅.

Depending on how Goddess of Fortune feels, we might get to talk tomorrow; or maybe it might be today, who knows 😛.

On the day to day basis, I specialize in creating high-quality modding tools and utilities that help
users and developers create game mods. My work spans from low-level reverse engineering and performance
optimization to user-facing applications and modding frameworks.

!!! info "My Journey"

    **From Gaming to Programming:** Started as a competitive gamer (e.g. was ranked #4 globally in Rocket League 1v1 in 2015 for a while),
    but transitioned to programming for more flexibility and better long term prospects.
    
    **Early Development:** Always tinkered with stuff, e.g. overclocked CPU at 9, modified Stock Android ROMs at 13 as a 'power user'.
    My first serious programming project was reverse engineering Sonic Heroes' object placement format in 2015.

    **Current Focus:** Building the next generation of modding infrastructure, including the [Reloaded3 Framework](https://reloaded-project.github.io/Reloaded-III/) and supporting ecosystem of libraries to let mod authors focus on making the best possible mods.

**Why I do this:** Game modding was my gateway into programming. I learned by experimenting, breaking things, and creating tools for games I loved.

I want to give others the same opportunity by reducing the barriers to entry for modding, especially
for niche games without established communities. I work every hour of every day to make the modding
ecosystem better for everyone, whether it's through the Nexus Mods App, my own projects, or contributions
to open source libraries.

For more details about my background and projects, visit [sewer56.dev](https://sewer56.dev).

## Item Classification

!!! info "Each item is classified as the following"

| Status                 | Meaning                                                                                               |
| ---------------------- | ----------------------------------------------------------------------------------------------------- |
| Unknown                | Unknown or not planned                                                                                |
| Shortlisted            | Internally noted (e.g. in Confluence) as possible future work item but work not yet planned or began. |
| Planned                | Company plans to do this in the future or the feature is in progress.                                 |

All classifications are to best of my knowledge at the time of writing.
For some of the projects, I'm already building them in my own time, every hour I can spare;
they are marked as the following:

| Status                 | Meaning                                                                                               |
| ---------------------- | ----------------------------------------------------------------------------------------------------- |
| In Progress (Weekends) | Working at this in my own time over weekends.                                                         |
| Planned (Weekends)     | Stuff I'll be working on in my own time.                                                              |

## Software Projects

!!! tip "Personal projects I'm building in my spare time"

    These are ambitious technical projects that would revolutionize the entire modding infrastructure.<br/>
    Each represents hundreds of hours of weekend development work (~30 hours a weekend).

Below are the ones I'm working on at this very moment, which would also benefit Nexus Mods.<br/>
I figured I'd put those first as it would give you the idea on the sort of things I specialize in(1).
{ .annotate }

1. (It's usually bleeding edge tech)

### [Lossless Texture Compression Library](./dxt-lossless-transform.md)

**Status:** In Progress (Own Project) • ~50% Complete

A library for losslessly transforming DXT/BC compressed texture files to reduce storage costs and improve performance.
This technology could significantly reduce file sizes for texture-heavy mods while maintaining perfect visual quality.

!!! note "Textures represent ~90% of space used by mods"

    This reduces the size of that 90% by around 9-15%, which translates to faster downloads, less disk
    space used and decreased operational costs for the website.

### [Nx2.0 Archive Format](./nx2.0.md)

**Status:** In Progress (Own Project) • ~50% Complete

A next-generation archive format designed specifically for mod distribution and high-performance asset loading.
Built to leverage modern storage hardware while being flexible enough for various use cases.

**Key Features:**

- ***File deduplication*** across mod versions: Don't store same archived files multiple times on Nexus Servers!
- ***Selective file downloads***: Download only the files you need, not the entire mod archive, *for any mod*.
- ***Delta updates***: Download only the changed bytes between mod versions.
- ***Streaming support***: Stream assets directly from the archive without fully extracting them.
- ***Improved Mod Author Experience***: Archive and upload mods in a literal fraction of the time compared to current formats.
- ***Optimized for a variety of use cases centered around modding***: Web Distribution, Game Asset Loading, Virtual FileSystem (VFS) etc.

### [A Better Modding Framework](./reloaded3.md)

**Status:** In Progress (Own Project) • Estimated Completion: 2028-2029 (hopefully)

A fully modular modding framework that provides everything needed to start modding any game without
reinventing the wheel. Aims to standardize modding infrastructure and bring revolutionary tech
across the entire modding ecosystem. (For every modder!)

The two projects above (and others, not named here) are parts of the larger
[Reloaded3](https://reloaded-project.github.io/Reloaded-III/) project.

## Site Feature Requests

!!! info "Features that would improve the Nexus Mods experience"

    These are practical improvements to make modding more accessible and efficient for everyone.

### User Experience Improvements

#### [Modular Mods are Painful](./modular-mods-are-painful.md)

**Status:** Unknown

Addresses the challenges of distributing and managing many small, modular mods on Nexus Mods,
particularly for multiplayer scenarios where users need to sync identical mod setups quickly.

### Download & Distribution Features

#### [Send Downloads to Specific Mod Manager](./nxm-handler.md)

**Status:** Unknown/Shortlisted

Allow the "Mod Manager Download" button for games not supported by Vortex, enabling users of other
mod managers to benefit from seamless downloads.

#### [Download Queue for Cross-Device Modding](./nxm-handler-queue.md)

**Status:** Unknown

Enable queuing downloads from mobile devices or other computers to be processed by your main gaming
setup, bridging the gap between mobile browsing and desktop modding.

#### [Batch Tiny File Downloads](./tiny-file-downloads.md)

**Status:** Unknown

Enable free users to download multiple small files (like translations) in batch, rather than visiting
each mod page individually. Particularly important for small modular translation packages.

#### [Release Branches](./release-branches.md)

**Status:** Unknown/Shortlisted

Support different release channels (stable, beta, alpha) for mods, allowing users to choose between
stability and cutting-edge features.

### Developer & Tool Integration

#### [Automatic Metadata Parsing](./metadata-parsing.md)

**Status:** Unknown/Shortlisted

Automatically parse mod metadata from standardized files (manifest.json, SubModule.xml, etc.) during
upload to improve categorization and compatibility checking.

#### [Collections Support for External Software](./collections-for-external-software.md)

**Status:** Unknown

Allow modding tools other than Vortex to create and share collections, making mod setups shareable
across different software ecosystems.

#### [Blob Storage for Modding Tools](./blob-storage.md)

**Status:** Unknown/Shortlisted

Provide small-scale data storage for modding tools to sync user preferences, configurations, and
other metadata across devices.

### Communication & Notifications

#### [External Notifications for Issue Tracker](./issue-tracker.md)

**Status:** Unknown

Send real-time notifications (webhooks, email) when users report issues with mods, enabling faster
response times from mod authors.

#### [Communicate API Changes](./communicate-api-changes.md)

**Status:** Unknown

Establish a proper communication channel for API changes and breaking updates to external tool developers,
preventing compatibility issues.