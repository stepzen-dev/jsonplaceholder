# jsonplaceholder


# Introduction

A StepZen schema for jsonplaceholder.typicode.com -- if you're interested in seeing how StepZen works with jsonplaceholder, a mocking service. 

## Getting Started
You'll need to create a [StepZen account](https://stepzen.com/request-invite) first. Once you've got that set up, [git clone](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone) this repository onto your machine and open the working directory.

Open your terminal and [install the StepZen CLI](https://stepzen.com/docs/quick-start). 

Run `git clone https://github.com/stepzen-samples/jsonplaceholder.git && cd jsonplaceholder`

After you've followed the prompts (you can accept the suggested endpoint name-- in my case it was `api/happy-bunny`) and installed the CLI, run `stepzen start`. 

A message similar to this will display:
```bash
Watching ~/jsonplaceholder for GraphQL changes
http://localhost:5000/api/happy-bunny
File changed: /Users/luciacerchie/jsonplaceholder/.git/config
Deploying to StepZen...... done
Successfully deployed api/happy-bunny at 9:00:07 AM
```
You'll see your StepZen Explorer pop up on your localhost:5000 address:
*include screenshot of your graphiql editor here with width set to 600* 
<img width="600" alt="Screen Shot 2021-07-01 at 9 08 20 AM" src="https://user-images.githubusercontent.com/54046179/124156000-f3a4d380-da4b-11eb-8f65-738a9cca6f8c.png">

In the left pane, copy and paste:

```graphql
query MyQuery {
  getAlbumPhotos(albumId: "1") {
    albumId
    title
  }
}
```
and you'll get json placeholder data in the response:

```json
{
  "data": {
    "getAlbumPhotos": [
      {
        "albumId": "1",
        "title": "accusamus beatae ad facilis cum similique qui sunt"
      },
      {
        "albumId": "1",
        "title": "reprehenderit est deserunt velit ipsam"
      },
      {
        "albumId": "1",
        "title": "officia porro iure quia iusto qui ipsa ut modi"
      },
      {
        "albumId": "1",
        "title": "culpa odio esse rerum omnis laboriosam voluptate repudiandae"
      },
      {
        "albumId": "1",
        "title": "natus nisi omnis corporis facere molestiae rerum in"
      },
```

## Learn More
You can learn more in the [StepZen documentation](https://stepzen.com/docs).

Reach out to us in [Discord](https://discord.gg/9k2VdPn2FR) if you need help. 

