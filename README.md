# This is WebScaleYesMark™, a version of [YesMark™](http://github.com/jeremycole/yesmark) that is designed for web scale.

WebScaleYesMark™ only requires one thing, `yes`. It works like this:

    yes "#" | mysql -c &

# Frequently Asked Questions

## How can I quickly run 24 threads of YesMark™?

You can achieve a faster spawning of WebScaleYesMark™ test threads with a simple shell for loop:

    for i in {1..24}; do yes "#" | mysql -c & done

## How can I tell what my performance is?

1. You know about `\s` right?
2. Use `mysqladmin -ri 1 extended-status | grep Questions`

## Why WebScaleYesMark™?

Because web scale.
