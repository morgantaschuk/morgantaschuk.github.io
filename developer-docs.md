# Developer Documentation

## First tag on the post is the sorting one

This is in the blog layout, but it appears on each filtered page based on the
first tag in the front matter. So if you want it in 'Writing', then put this in
the front matter

    tags: writing all-the-other-tags

## Adding instasgraam photos

When making a post with an instagram photo, use this magic resolving URL:
"https://instagram.com/p/XXXX/media/?size=l" where XXXX is the unique code from
instagram. The size can be 't' for thumbnail, 'm' for medium, or 'l' for large.
See [Developer Docs on
embedding](https://www.instagram.com/developer/embedding/) for more deets.


