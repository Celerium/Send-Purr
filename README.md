# Send-Purr

The Send-Purr script sends a cat image & fact to a Teams channel using a Teams webhook connector URI.

- Various filters are in place to try and prevent any inappropriate images from being sent.

An image is randomly selected from a random cat subreddit. Cat facts are pulled from the catfact.ninja API
When the r/Chonkers subreddit is used, the Teams post will be formatting to accommodate for the chonks size.

---

## Send-Purr

![Send-Purr](https://raw.githubusercontent.com/Celerium/Send-Purr/main/.github/Celerium-Send-Purr-Example001.png)

## Initial Setup & Running

1. Teams Channel > Connectors > Incoming Webhook
2. Give the Webhook a name & logo
    - Create the Webhook
4. Copy the URI
    - The URI is how you tell the script what teams channel to send posts to.

---

```posh
    .\Send-Purr.ps1 -TeamsURI 'https://outlook.office.com/webhook/123/123/123/.....'
```

Using the defined webhooks connector URI a random dad joke is sent to the webhooks Teams channel.

No output is displayed to the console.
Using the -Verbose option will give you a basic display output


## Help :blue_book:

  - Help info and a list of parameters can be found by running `Get-Help .\Send-Purr.ps1`, such as:

```posh
Get-Help .\Send-Purr.ps1
Get-Help .\Send-Purr.ps1 -Full
```

---