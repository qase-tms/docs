---
title: "How to use Environments in Qase"
slug: "environments-1"
hidden: true
createdAt: "2023-02-24T12:53:22.196Z"
updatedAt: "2023-02-27T18:47:35.491Z"
---
Environments in a test case management system are an additional entity which allows you to represent your real-life infrastructure environments and then specify which of the environment a Test Run should be executed in.
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2F7XLLVD8c8x4%3Ffeature%3Doembed&display_name=YouTube&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D7XLLVD8c8x4&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2F7XLLVD8c8x4%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"854\" height=\"480\" scrolling=\"no\" title=\"YouTube embed\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=7XLLVD8c8x4",
  "title": "Using Qase / Execution: Environments",
  "favicon": "https://www.google.com/favicon.ico",
  "image": "https://i.ytimg.com/vi/7XLLVD8c8x4/hqdefault.jpg"
}
[/block]
In order to create an environment in Qase, go to the Project's "Environments" tab, then click "Create new environment":

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/eaaf51c-O-owFkooQ-imTeIlM6emC4sjQn6tYw1jHOsbvUEghH72IkMOqCxILv1Sl2D1X549ArTMZDDwf7eQ2oey2mIJfr-cwBiN28xHNhoy_O9cWBI4WVB9lG7rLQyDsCXbnRZQznSER-3avyc6PWn-7USGPq-gP3wZLEsE40-YpceQBbJBc6b05o9jqXfExQ",
        "O-owFkooQ-imTeIlM6emC4sjQn6tYw1jHOsbvUEghH72IkMOqCxILv1Sl2D1X549ArTMZDDwf7eQ2oey2mIJfr-cwBiN28xHNhoy_O9cWBI4WVB9lG7rLQyDsCXbnRZQznSER-3avyc6PWn-7USGPq-gP3wZLEsE40-YpceQBbJBc6b05o9jqXfExQ",
        1002,
        599,
        "#000000"
      ]
    }
  ]
}
[/block]
Define the environment's properties:


[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e66307f-MlkcrAMuSeBNKF3o3hPq5TmLJbst8p9hjkxdBvkclIhP3i6ZhZrdB3M7WUg-JOHDrCq1ZAFmCX2qnCfT2kmx3jZ4ohrdm43uzFcPon0wkr_Z8VYWqcZlF_sBUqonRnCeNkOq8Wja0KGl0FZZpYW9HlqQtWrGBn_xjOvu6WIcLNkOHaWIWNPEA0wbNg",
        "MlkcrAMuSeBNKF3o3hPq5TmLJbst8p9hjkxdBvkclIhP3i6ZhZrdB3M7WUg-JOHDrCq1ZAFmCX2qnCfT2kmx3jZ4ohrdm43uzFcPon0wkr_Z8VYWqcZlF_sBUqonRnCeNkOq8Wja0KGl0FZZpYW9HlqQtWrGBn_xjOvu6WIcLNkOHaWIWNPEA0wbNg",
        799,
        607,
        "#000000"
      ]
    }
  ]
}
[/block]
Insert a Slug: This is a mandatory field of a URL-friendly shortened version of the title (i.e., “prod”)

Input a Description: This is an optional field for extra context about the environment and what it's to be used for

Include a Host: This is another optional field and should be the URL address of the environment (as a reference)


Once completed, your new environment can be used as a property of a Test run when creating or editing Test runs:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6376c7b-twVZdOyHtINDwdB1JZ5i3GbxP4v7COQnj14p5Bnr3xuk5aIV-eA0gTJ5pvbWw99gL3BfH0FzX34MDDKfOKFNGniL0aMt3tlOUI7246KgAapgeq0zUdqrQ0_-mlccBkiBdUMjd4rCyiRvHki7G-b0RpC2OB-L8OGs2ov0sL9VvlFukg6UzoMbtzzSdg",
        "twVZdOyHtINDwdB1JZ5i3GbxP4v7COQnj14p5Bnr3xuk5aIV-eA0gTJ5pvbWw99gL3BfH0FzX34MDDKfOKFNGniL0aMt3tlOUI7246KgAapgeq0zUdqrQ0_-mlccBkiBdUMjd4rCyiRvHki7G-b0RpC2OB-L8OGs2ov0sL9VvlFukg6UzoMbtzzSdg",
        1336,
        602,
        "#000000"
      ]
    }
  ]
}
[/block]