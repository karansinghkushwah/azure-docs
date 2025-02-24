---
title: Azure Event Grid - Subscribe to SAP events
description: This article explains how to subscribe to events published by SAP.
ms.topic: how-to
ms.date: 10/25/2022
---

# Subscribe to events published by SAP
This article describes steps to subscribe to events published by an SAP S/4HANA system.

## High-level steps

The common steps to subscribe to events published by any partner, including SAP, are described in [subscribe to partner events](subscribe-to-partner-events.md). For your quick reference, the steps are provided again here with the addition of a step to make sure that your SAP system has the required components. This article deals with steps 1 and 3.

1. [Ensure you meet all prerequisites](#prerequisites).
1. Register the Event Grid resource provider with your Azure subscription.
1. Authorize partner to create a partner topic in your resource group.
1. [Enable SAP S/4HANA events to flow to a partner topic](#enable-events-to-flow-to-your-partner-topic).
1. Activate partner topic so that your events start flowing to your partner topic.
1. Subscribe to events.

## Prerequisites

Following are the prerequisites that your system needs to meet before attempting to configure your SAP system to send events to Azure Event Grid.

1. SAP S/4HANA system (on-premises) version 2020 or later.
1. SAP's [Business Technology Platform](https://www.sap.com/products/technology-platform.html)(BTP).
1. On the Business Technology Platform, [SAP Event Mesh](https://help.sap.com/docs/SAP_EM/bf82e6b26456494cbdd197057c09979f/df532e8735eb4322b00bfc7e42f84e8d.html) is enabled.

If you have any questions, contact us at <a href="mailto:ask-grid-and-ms-sap@microsoft.com">ask-grid-and-ms-sap@microsoft.com</a>

## Enable events to flow to your partner topic

SAP's capability to send events to Azure Event Grid is available through SAP's [beta program](https://influence.sap.com/sap/ino/#campaign/3314). Using this program, you can let SAP know about your desire to have your S4/HANA events available on Azure. You can find the SAP's announcement of this new feature [here](https://blogs.sap.com/2022/10/11/sap-event-mesh-event-bridge-to-microsoft-azure-to-go-beta/). Through SAP's Beta program, you'll be provided with the documentation on how to configure your SAP S4/HANA system to flow events to Event Grid. At at that point, you may proceed with the next step in the process described in the [High-level steps](#high-level-steps) section.

SAP's BETA program started in October 2022 and will last a couple of months. Thereafter, the feature will be released by SAP as a generally available (GA) capability. Event Grid's capability to receive events from a partner, like SAP, is already a GA feature.

If you have any questions, you can contact us at <a href="mailto:ask-grid-and-ms-sap@microsoft.com">ask-grid-and-ms-sap@microsoft.com</a>.

## Next steps
See [subscribe to partner events](subscribe-to-partner-events.md).