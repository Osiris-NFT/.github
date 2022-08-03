[![nfts.jpg](https://i.postimg.cc/T1Fm0cbV/red.jpg)](https://postimg.cc/2LdV8h2y)

Osiris is a platform where anyone can generate, share and/or sell NFTs in order to help small creators and beginners post their creations by giving them a very friendly and guided user experience.

## Architecture
The application follow a microservices architecture by running multiple small services on the cloud and have a full and automated CI/CD pipeline. Every repository represents one service that is fully independant from others. Osiris NFT is only available on Android.

## Workflow
Every services have their own unique GitHub Action script that build and push their images into a docker repository. A repository dispatch trigger the GitHub Action of the *Deployment* repository composed with multiple configuration and testing files, deploy the updated application on Google Cloud, and then run multiple tests on each API endpoints.


*School project, ***ISEN Yncrea Méditerranée, Toulon**.**
