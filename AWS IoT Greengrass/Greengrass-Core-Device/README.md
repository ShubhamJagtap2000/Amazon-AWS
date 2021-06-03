# Greengrass Core Device

- A device that runs the AWS IoT Greengrass Core software. A Greengrass core device is an AWS IoT thing. You can add multiple core devices to AWS IoT thing groups to create groups of Greengrass core devices. 

### Greengrass component

- A software module that is deployed to and runs on a Greengrass core device. All software that is developed and deployed with AWS IoT Greengrass is modeled as a component.
- AWS IoT Greengrass provides pre-built public components that provide features and functionality that you can use in your applications.
- You can also develop your own custom components, on your local device or in the cloud. After you develop a custom component, you can use the AWS IoT Greengrass cloud service to deploy it to single or multiple core devices.
- You can create a custom component and deploy that component to a core device. When you do, the core device downloads the following resources to run the component: 

  * **1. Recipe:** A JSON or YAML file that describes the software module by defining component details, configuration, and parameters.
 
  * **2. Artifact:** The source code, binaries, or scripts that define the software that will run on your device. You can create artifacts from scratch, or you can create a component using a Lambda function, a Docker container, or a custom runtime.
  
  * **3. Dependency:** The relationship between components that enables you to enforce automatic updates or restarts of dependent components. For example, you can have a secure message processing component dependent on an encryption component. This ensures that any updates to the encryption component automatically update and restart the message processing component. 
