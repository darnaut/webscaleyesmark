# This is WebScaleYesMark™, the world's most advanced Open Source benchmarking platform.

WebScaleYesMark™ only requires one thing, `yes`. It works like this:

    yes "#" | mysql -c &

# Frequently Asked Questions

## How can I quickly run 16 threads of YesMark™?

You can achieve a faster spawning of WebScaleYesMark™ test threads with a simple shell for loop:

    for i in {1..16}; do yes "#" | mysql -c & done

## How can I tell what my performance is?

1. You know about `\s` right?
2. Use `mysqladmin -ri 1 extended-status | grep Questions`

## Why WebScaleYesMark™?

Because web scale.
