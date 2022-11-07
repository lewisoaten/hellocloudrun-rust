# CloudRun Rust Example

## Acknowledgements

These instructions are nothing without the excellent [Hello Cloud Run with Python](https://codelabs.developers.google.com/codelabs/cloud-run-hello-python3) Code Lab. Written by Laurent Picard (:octocat: [@PicardParis](https://github.com/PicardParis)).

The code itself is taken from Knative's [Rust Code Sample](https://github.com/knative/docs/tree/main/code-samples/community/serving/helloworld-rust). Just a bit of minor version bumping required. I have also included a lockfile to avoid this issue when the GitHub archeologists attempt to resurrect this code.

## Introduciton

This is a sample Rust application intended for learning how ot use Google Cloud Run with Rust. This has been developed for the [Google Developer Group Hants & Surrey](https://www.meetup.com/google-developer-group-hants-surrey/) event [10th November 2022: Unleash the power of Rust and Cloud Run](https://www.meetup.com/google-developer-group-hants-surrey/events/288970824/).

## Instructions

1. Set up of the project can be done using the [Hello Cloud Run with Python](https://codelabs.developers.google.com/codelabs/cloud-run-hello-python3) code lab stages 1-3.
2. Clone this repo.
3. Deploy to Cloud Run: `gcloud beta run deploy hellocloudrun-rust --source . --platform managed --region europe-west2 --allow-unauthenticated`
4. Check your service URL: `gcloud run services describe hellocloudrun-rust --platform managed --region europe-west2 --format "value(status.url)"`
5. Clean up of the project can be done using the [Hello Cloud Run with Python](https://codelabs.developers.google.com/codelabs/cloud-run-hello-python3) code lab stage 7.
