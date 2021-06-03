# AWS IoT Greengrass

### All notes are taken from : Official Developer Guide [here](https://docs.aws.amazon.com/greengrass/v2/developerguide/how-it-works.html) 

## What is it?

- AWS IoT Greengrass is an open source Internet of Things (IoT) edge runtime and cloud service that helps you build, deploy and manage IoT applications on your devices.

## What it does?

- You can use AWS IoT Greengrass to build software that enables your devices to act locally on the data that they generate, run predictions based on machine learning models, and filter and aggregate device data.

## How an AWS IoT Greengrass device interacts with the AWS Cloud?

- AWS IoT Greengrass enables your devices to collect and analyze data closer to where that data is generated, react autonomously to local events, and communicate securely with other devices on the local network.
- Greengrass devices can also communicate securely with AWS IoT Core and export IoT data to the AWS Cloud. You can use AWS IoT Greengrass to build edge applications using pre-built software modules, called components, that can connect your edge devices to AWS services or third-party services.
- Refer this example,

![greengrass-overview](https://user-images.githubusercontent.com/63872951/120613434-df34e180-c473-11eb-93e7-16ee6276d074.png)

## How AWS IoT Greengrass works?

- AWS IoT Greengrass enables local execution of AWS Lambda functions, Docker containers, native OS processes, or custom runtimes of your choice. 
- AWS IoT Greengrass provides pre-built software modules called components that let you easily extend edge device functionality. AWS IoT Greengrass components enable you to connect to AWS services and third-party applications at the edge. After you develop your IoT applications, AWS IoT Greengrass enables you to remotely deploy, configure, and manage those applications on your fleet of devices in the field. 
- The following example shows how an AWS IoT Greengrass device interacts with the AWS IoT Greengrass cloud service and other AWS services in the AWS Cloud,

![how-it-works](https://user-images.githubusercontent.com/63872951/120614214-a0ebf200-c474-11eb-8957-9f5629ff1e8f.png)

## Key concepts for AWS IoT Greengrass

### 1.Greengrass core device

- A device that runs the AWS IoT Greengrass Core software. A Greengrass core device is an AWS IoT thing. You can add multiple core devices to AWS IoT thing groups to create groups of Greengrass core devices. 

### Greengrass component

- A software module that is deployed to and runs on a Greengrass core device. All software that is developed and deployed with AWS IoT Greengrass is modeled as a component.
- AWS IoT Greengrass provides pre-built public components that provide features and functionality that you can use in your applications.
- You can also develop your own custom components, on your local device or in the cloud. After you develop a custom component, you can use the AWS IoT Greengrass cloud service to deploy it to single or multiple core devices.
- You can create a custom component and deploy that component to a core device. When you do, the core device downloads the following resources to run the component: 
  * **1. Recipe:** A JSON or YAML file that describes the software module by defining component details, configuration, and parameters.
  * **2. Artifact:** The source code, binaries, or scripts that define the software that will run on your device. You can create artifacts from scratch, or you can create a component using a Lambda function, a Docker container, or a custom runtime. 
  * **3. Dependency:** The relationship between components that enables you to enforce automatic updates or restarts of dependent components. For example, you can have a secure message processing component dependent on an encryption component. This ensures that any updates to the encryption component automatically update and restart the message processing component. 
