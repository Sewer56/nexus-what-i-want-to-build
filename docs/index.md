# What does Seweryn want to build?

!!! question "What would you build if you had a magic wand?"

    *Is what the Chosen Ones said.*

Having had a lot of thoughts for a long time, and never the proper time to compile them, I might just
take the time to list some of them here. 😉

This is my own wishlist, some of the items here are things I have already started working on
(alone, in my own time) and some are just ideas for the site itself that I think would be essential to have.

## About Me

Hi, I'm Seweryn (aka Sewer56), a "full-stack modder" and open source library author working as one of the guys at the App Team.
Depending on how Goddess of Fortune feels, we might get to talk tomorrow; or maybe it might be today, who knows 😛.

I specialize in creating high-quality modding tools and utilities that help users and developers create game mods.
My work spans from low-level reverse engineering and performance optimization to user-facing applications and modding frameworks.

!!! info "My Journey"

    **From Gaming to Programming:** Started as a competitive gamer (was ranked #4 globally in Rocket League 1v1 in 2015 for a while), but transitioned to programming for sustainability and flexibility.
    
    **Early Development:** Began with Android ROM development at age 13, creating custom ROMs like Gin2JellyBean Extended and OxySlim. My first serious programming project was reverse engineering Sonic Heroes' object placement format in 2015.
    
    **Current Focus:** Building the next generation of modding infrastructure, including the [Reloaded3 Framework](https://reloaded-project.github.io/Reloaded-III/) and supporting ecosystem of libraries.

**Why I do this:** Game modding was my gateway into programming. I learned by experimenting, breaking things, and creating tools for games I loved. I want to give others the same opportunity by reducing the barriers to entry for modding, especially for niche games without established communities. I work every hour of every day to make the modding ecosystem better for everyone, whether it's through the Nexus Mods App, my own projects, or contributions to open source libraries.

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

    These are ambitious technical projects that would revolutionize the entire modding infrastructure.

    Each represents hundreds of hours of weekend development work.

### [Lossless Texture Compression Library](./dxt-lossless-transform.md)

**Status:** In Progress (Own Project) • ~50% Complete

A library for losslessly transforming DXT/BC compressed texture files to reduce storage costs and improve performance.
This technology could significantly reduce file sizes for texture-heavy mods while maintaining perfect visual quality.

!!! note "Textures represent ~90% of space used by mods"

    This makes mods use up to 15% less space on disk, which translates to 15% faster downloads and
    server resources used.

### [Nx2.0 Archive Format](./nx2.0.md)

**Status:** In Progress (Own Project) • ~50% Complete

A next-generation archive format designed specifically for mod distribution and high-performance asset loading.
Built to leverage modern storage hardware while being flexible enough for various use cases.

**Key Features:**

- File deduplication across mod versions: Don't store same file multiple times on CDN!
- Selective file downloads: Download only the files you need, not the entire mod archive
- Delta updates: Download only the changed bytes between mod versions.
- Optimized for both web distribution and local storage

### [A Better Modding Framework](./reloaded3.md)

**Status:** In Progress (Own Project) • Estimated Completion: 2028

A fully modular modding framework that provides everything needed to start modding any game without
reinventing the wheel. Aims to standardize modding infrastructure across the entire ecosystem.

## Site Feature Requests

!!! info "Features that would improve the Nexus Mods experience"

    These are practical improvements to make modding more accessible and efficient for everyone.

### Download & Distribution Features

#### [Send Downloads to Specific Mod Manager](./nxm-handler.md)

**Status:** Unknown/Shortlisted

Allow the "Mod Manager Download" button for games not supported by Vortex, enabling users of other
mod managers to benefit from seamless downloads.

#### [Batch Tiny File Downloads](./tiny-file-downloads.md)

**Status:** Unknown

Enable free users to download multiple small files (like translations) in batch, rather than visiting
each mod page individually. Particularly important for comprehensive translation packages.

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