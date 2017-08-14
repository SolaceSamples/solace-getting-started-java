[![Build Status](https://travis-ci.org/SolaceSamples/solace-samples-java.svg?branch=master)](https://travis-ci.org/SolaceSamples/solace-samples-java)

# Getting Started Examples
## Solace Java API (JCSMP)

These tutorials will get you to up to speed and quickly sending messages with Solace technology.

Before you begin, you need access to Solace Messaging. Here are a few options of how you can get access:

### Option 1: Use DataGo

* Follow these instructions to quickly spin up a cloud based Solace messaging service for your applications.

### Option 2: Start a Solace VMR

* For instructions on how to start the Solace VMR in leading Clouds, Container Platforms or Hypervisors see the "Set up a VMR" tutorials which outline where to download and and how to install the software.

### Option 3: Get access to a Solace appliance

* Contact your Solace appliance administrators and obtain the following:
    * A Solace Message-VPN where you can produce and consume direct and persistent messages
    * The host name or IP address of the Solace appliance hosting your Message-VPN
    * A username and password to access the Solace appliance

## Contents

This repository contains code and matching tutorial walk throughs for five different basic Solace messaging patterns. For a nice introduction to the Solace API and associated tutorials, check out the [tutorials home page](https://solacesamples.github.io/solace-samples-java/).

See the individual tutorials for details:

* [Publish/Subscribe](https://solacesamples.github.io/solace-samples-java/publish-subscribe): Learn how to set up pub/sub messaging on a Solace VMR.
* [Persistence](https://solacesamples.github.io/solace-samples-java/persistence-with-queues): Learn how to set up persistence for guaranteed delivery.
* [Request/Reply](https://solacesamples.github.io/solace-samples-java/request-reply): Learn how to set up request/reply messaging.
* [Confirmed Delivery](https://solacesamples.github.io/solace-samples-java/confirmed-delivery): Learn how to confirm that your messages are received by a Solace message router.
* [Topic to Queue Mapping](https://solacesamples.github.io/solace-samples-java/topic-to-queue-mapping): Learn how to map existing topics to Solace queues.

## Prerequisites

This tutorial requires the Solace Java API library. Download the Java API library to your computer from [here](http://dev.solace.com/downloads/).

## Build the Samples

Just clone and build. For example:

  1. clone this GitHub repository
  1. `./gradlew assemble`

## Running the Samples

To try individual samples, build the project from source and then run samples like the following:

    ./build/staged/bin/topicPublisher <host:port> <message-vpn> <client-username> <client-password>

The individual tutorials linked above provide full details which can walk you through the samples, what they do, and how to correctly run them to explore Solace messaging.

## Exploring the Samples

### Setting up your preferred IDE

Using a modern Java IDE provides cool productivity features like auto-completion, on-the-fly compilation, assisted refactoring and debugging which can be useful when you're exploring the samples and even modifying the samples. Follow the steps below for your preferred IDE.

#### Using Eclipse

To generate Eclipse metadata (.classpath and .project files), do the following:

    ./gradlew eclipse

Once complete, you may then import the projects into Eclipse as usual:

 *File -> Import -> Existing projects into workspace*

Browse to the *'solace-samples-java'* root directory. All projects should import
free of errors.

#### Using IntelliJ IDEA

To generate IDEA metadata (.iml and .ipr files), do the following:

    ./gradlew idea

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

See the list of [contributors](https://github.com/SolaceSamples/solace-samples-java/contributors) who participated in this project.

## License

This project is licensed under the Apache License, Version 2.0. - See the [LICENSE](LICENSE) file for details.

## Resources

For more information try these resources:

- The Solace Developer Portal website at: http://dev.solace.com
- Get a better understanding of [Solace technology](http://dev.solace.com/tech/).
- Check out the [Solace blog](http://dev.solace.com/blog/) for other interesting discussions around Solace technology
- Ask the [Solace community.](http://dev.solace.com/community/)
