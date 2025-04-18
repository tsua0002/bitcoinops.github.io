---
title: Unannounced channels

## Optional.  An entry will be added to the topics index for each alias
title-aliases:
  - Private channels

## Required.  At least one category to which this topic belongs.  See
## schema for options
topic-categories:
  - Lightning Network

## Required.  Use Markdown formatting.  Only one paragraph.  No links allowed.
## Should be less than 500 characters
excerpt: >
  **Unannounced channels** are LN channels that are not advertised to
  the network for use in routing.

## Optional.  Produces a Markdown link with either "[title][]" or
## "[title](link)"
#primary_sources:
#    - title: Test
#    - title: Example
#      link: https://example.com

## Optional.  Each entry requires "title", "url", and "date".  May also use "feature:
## true" to bold entry
optech_mentions:
  - title: "LND #1944 tweaks `sendtoroute` RPC to allow routing via private channels"
    url: /en/newsletters/2018/11/13/#lnd-1944

  - title: "C-Lightning #2230 adds a `private` flag to the `listpeers` RPC"
    url: /en/newsletters/2019/01/15/#c-lightning-2230

  - title: "C-Lightning #2234 adds route hints for private channels to `invoice` RPC"
    url: /en/newsletters/2019/01/22/#c-lightning-2234

  - title: "Talk about LN topology and lack of public info about unannounced channels"
    url: /en/newsletters/2019/09/18/#lightning-network-topology

  - title: "C-Lightning #3351 enhances `invoice` RPC for private channels"
    url: /en/newsletters/2020/01/08/#c-lightning-3351

  - title: "Eclair #1283 allows multipath payments to traverse unannounced channels"
    url: /en/newsletters/2020/01/22/#eclair-1283

  - title: "Breaking the link between UTXOs and unannounced channels"
    url: /en/newsletters/2020/01/29/#breaking-the-link-between-utxos-and-unannounced-channels

  - title: "C-Lightning #3600 adds blinded paths to improve unannounced channel privacy"
    url: /en/newsletters/2020/04/08/#c-lightning-3600

  - title: "C-Lighting #3623 improves unannounced channel privacy when routing payments"
    url: /en/newsletters/2020/04/22/#c-lightning-3623

  - title: "C-Lightning #4611 updates the `keysend` RPC to support unannounced channels"
    url: /en/newsletters/2021/07/21/#c-lightning-4611

  - title: "LND v0.17.0-beta ships with experimental support for unannounced taproot and MuSig2 LN channels"
    url: /en/newsletters/2023/10/04/#lnd-v0-17-0-beta

  - title: "Core Lightning #6869 updates the listchannels RPC to no longer list unannounced channels"
    url: /en/newsletters/2024/01/03/#core-lightning-6869

## Optional.  Same format as "primary_sources" above
see_also:
  - title: Blinded paths
    link: topic rv routing
---
Most unannounced channels are believed to belong to users that simply
don't intend to route payments, such as users of mobile clients that
aren't always online to route payments.

An alternative name is **private channels,** but there's contention
between experts about whether the channels [improve privacy][privacy
in pcns] or [not][unpublished channels delenda est], so it may be
preferable to use the universally accepted name "unannounced
channels."

{% include references.md %}
[privacy in pcns]: https://arxiv.org/pdf/1909.02717.pdf "Section 4.1: endpoint uncertainty"
[unpublished channels delenda est]: https://gnusha.org/url/https://lists.linuxfoundation.org/pipermail/lightning-dev/2019-December/002408.html
