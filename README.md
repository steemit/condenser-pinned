## To modify a pinned post:

1. Open [pinned-posts.json](https://github.com/steemit/condenser-pinned/blob/master/pinned-posts.json)
2. Tap the pencil icon to edit
3. Insert the URL of the post you want to pin within the `[]`

For example, to pin a post:

    "pinned_posts": [
        "/steem/@steemitblog/smt-development-update-6"
      ]
    }

To replace a pinned post, simply edit the URL above.

To remove a pinned post (so no pinned post displays), remove the URL, e.g.

    {
      "pinned_posts": [
        
      ]
    }```

## Deploy changes to website

**Deploy to steemitdev.com**

After that, it needs to be deployed to the website. This can be done via Slack.

To test the deploy on [steemitdev.com](http://steemitdev.com/):

In the Slack channel #eng-dev, type:

`watt deploy condenser latest to dev`

It should appear on [steemitdev.com](http://steemitdev.com/).

**Deploy to steemit.com**

Once that works, deploy to [steemit.com](http://steemit.com/)
In the Slack channel #eng-production, type:

`watt deploy condenser latest to prod`
