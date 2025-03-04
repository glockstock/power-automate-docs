---
title: Understand the cloud flows designer
description: Learn about the components in the cloud flows designer.
suite: flow
author: kisubedi
contributors:
 - kisubedi
 - v-aangie
ms.subservice: cloud-flow
ms.topic: overview
ms.date: 10/02/2023
ms.author: kisubedi
search.audienceType: 
  - flowmaker
  - enduser
ms.reviewer: angieandrews
---

# Understand the cloud flows designer

You can create, configure, and customize your cloud flows with the classic designer or the cloud flows designer. For a description of the types of cloud flows, go to [Overview of cloud flows](overview-cloud.md).

> [!NOTE]
> Here are some visual queues that tell you that you're using the cloud flows designer (not the classic designer):
> - The cards in the flow are small.
> - The standalone action configuration pane appears on the left when you select a card.
>
> More information: [Identify differences between the classic designer and the cloud flows designer](#identify-differences-between-the-classic-designer-and-the-cloud-flows-designer)

The following screenshot shows the features of the AI-powered cloud flows designer.

:::image type="content" source="media/flows-designer/designer-overview-numbers-borders.png" alt-text="Screenshot of the cloud flows designer with Copilot.":::

Legend:

1. **Left arrow button**: Return to the previous page.
1. [**Send feedback button**](#send-feedback): Send us feedback about your flow creation experience or general comments about the AI-powered designer.
1. **Action/trigger name**: The action or trigger card that is selected in your flow in the center of the page.
1. [**More commands button**](#more-commands): Add a note to the selected card, or delete the card.
1. **Collapse button**: Hide the pane. When the pane is collapsed, the **Expand** button (**\>\>**) appears in the upper-left corner. Select it to show the pane again.
1. [**Copilot button**](get-started-with-copilot.md): Show or hide the Copilot pane. The Copilot pane appears by default when the AI-powered designer opens.
1. [**Save button**](#save-button): Save your flow.
1. [**Test button**](#test-button): Test your flow to make sure that it works as you intended.
1. [**Action configuration pane**](#action-configuration-pane): After you select an action card to configure on the canvas, the action configuration pane opens on the left side of the AI-powered designer.
1. [**Canvas**](#canvas): The canvas is where you build your flow. It's free-flowing and therefore allows for easier navigation.
1. [**Copilot pane**](get-started-with-copilot.md): Copilot stays with you during your flow editing and fit-and-finish journey. It can help you update and make changes to your flow, based on your conversational-style prompt. It can also help answer flow-related and product-related questions.

## Send feedback

We want to hear from you to help us measure and improve our impact. To provide your feedback, select **Send Feedback**, answer the three questions in the feedback form that opens, and then select **Submit**.

:::image type="content" source="media/flows-designer/feedback.png" alt-text="Screenshot of the feedback form.":::

## More commands

Select the **More commands** (**&hellip;**) button to add a note to the selected card in your flow, or to delete the card. Select **Add a note** to describe the purpose of the card in your flow. After you add a note, a note symbol appears in the lower right of the card. Hover over this symbol to view the note.

:::image type="content" source="media/flows-designer/designer-note.png" alt-text="Screenshot that shows a note being added.":::

## Save button

Select **Save** to save your flow. If there are no errors, the message, *"Your flow is ready to go. We recommend you test it"* appears in the upper left with a green check.

:::image type="content" source="media/flows-designer/designer-save.png" alt-text="Screenshot of a successful save.":::

If an error is found, a description of the error and a red *X* appear in the upper left. The following screenshot shows an example of an error message.

:::image type="content" source="media/flows-designer/designer-error.png" alt-text="Screenshot of an error message.":::

The error also appears on the card that caused the error in your flow. Correct the error, and then select **Save** again.

When there are no errors, your next step should be to test your flow.

## Test button

After your flow is saved successfully, **Test** becomes active. To test your flow, select **Test** > After your flow is successfully saved, the **Test** button becomes available. To test your flow, select **Test**, select the **Manually** option, and then select **Test**.

:::image type="content" source="media/flows-designer/test-manually.png" alt-text="Screenshot of the option for manually testing your flow.":::

Instructions appear and tell you what you must do to test your flow. The following screenshot shows an example of an instructional message.

:::image type="content" source="media/flows-designer/test-prompt.png" alt-text="Screenshot of instructions that tell you how to test your flow.":::

Follow the instructions to test your flow. In this example, you must send an email. The flow test then runs. When the test has finished running, a green check mark appears on each card, together with the number of seconds that it took to be processed.

:::image type="content" source="media/flows-designer/test-result.png" alt-text="Screenshot of test results.":::

Testing is part of the planning for a Power Automate project. To learn more, go to [Introduction: Planning a Power Automate project](guidance/planning/introduction.md).

## Action configuration pane

Use the action configuration pane to customize parameters, settings, and code for the selected card in your flow.

### Parameters

On the **Parameters** tab, you can use the blue **Insert token** (lightning bolt) and **Insert expression** (***fx***) buttons next to the **Inputs** field to quickly enter values for the selected action card.

:::image type="content" source="media/flows-designer/skittles.png" alt-text="Screenshot of the Insert token and Insert expression buttons on the Parameters tab in the action configuration pane.":::

To insert a dynamic token into the **Inputs** field, select the **Insert token** (lightning bolt) button. In the pop-up window that opens, search for or scroll to find the tokens that you can use. After you select a token, it appears in the **Inputs** field.

To insert an expression into the **Inputs** field, select the **Insert expression** (***fx***) button. In the pop-up window that opens, select a function to start your expression. To complete your expression, place the cursor in the function, and then select **Dynamic content**. Search for or select the content/tokens to add, and then select **Add**. Your completed expression appears in the **Inputs** field.

To learn more about expressions, go to [Reference guide to workflow expression functions](/azure/logic-apps/workflow-definition-language-functions-reference).

Alternatively, use the keyboard to enter a slash (**/**) in the **Inputs** field. Then select the dynamic content/token and expression pop-ups.

### Settings

On the **Settings** tab, you can set the action time-out, network retry policy, how an action should run, security input and output, and tracking properties. The following table provides a description of the settings.

| Setting | Description |
|---------|-------------|
| General | In the **Action Timeout** field, set the maximum duration between retries and asynchronous responses for the selected action. This setting doesn't change the request time-out of a single request. |
| Networking | In the **Retry Policy** field, select a retry policy for intermittent failures. The default setting is an exponential interval policy that is set to retry four times. You can also set your own exponential or fixed interval settings, or choose none at all. |
| Run After | In the **Run After** field, configure how an action should run after the execution of any of the preceding flow actions. For example, you can choose to run an action after the preceding action runs successfully, times out, skips, or fails. |
| Security | Use the **Secure inputs** and **Secure outputs** toggles to turn the operations, and references of output properties, on or off. |
| Tracking | Set the key and value of tracked properties.

### Code

To view the code behind any card in your flow, select the card on the canvas, and then select **Code View** in the action configuration pane. As you customize the code on the [Parameters](#parameters) tab, you can view the new code on the **Code View** tab.

The following screenshot shows an example of the code for the **Compose** action card.

:::image type="content" source="media/flows-designer/compose.png" alt-text="Screenshot of the code view of the Compose action card.":::

## Canvas

For easy navigation, you can drag your flow on the canvas. You configure the actions of each card in the action configuration pane on the left. The cards on the canvas are compact to allow for easy visibility and navigation, especially in large flows.

### Drop zones

The canvas contains AI-powered designer drop zones to help you easily drag cloud flow actions. The drop zones are indicated by blue dashed lines.

:::image type="content" source="media/flows-designer/drop-zone.png" alt-text="Screenshot of an action card and a drop-zone.":::

### Zoom buttons

Depending on the size and complexity of your flow, you might want to adjust its size on the canvas as you're building it. Use the zoom buttons to zoom in, zoom out, fit to screen, and toggle a *minimap*. The buttons appear when the Action configuration pane is closed.

The bottom button is for the minimap. Use it to focus on a specific section of a large flow.

:::image type="content" source="media/flows-designer/zoom-controls.png" alt-text="Screenshot of the four zoom buttons.":::

## Identify differences between the classic designer and the cloud flows designer

To quickly identify which designer version you're using, ask yourself the following questions:

- Are the action cards on the flow small or large?
- Is the action configuration pane inline or in a separate pane?

The cloud flows designer has smaller cards to facilitate easy navigation. It also has a standalone action configuration pane on the left.

## Limitation

You might notice that some functionalities that were in the classic designer aren't available in the cloud flows designer. For example, the designer doesn't support non-Open API flows (Peek code on an action and if you see `_methods_` parameter, the flow is a non-open API flow), and constructs such as some hybrid triggers (for a selected message (v2 Teams), TeamsoncomposeMesage (teams), Teams card trigger, Microsoft 365 Compliance Connector), a comment, Power Pages connector, or a Power Apps v1 trigger in your flow.

If you want to work with missing functionalities in the designer, select **Switch to classic designer** on the menu in the cloud flows designer.

> [!NOTE]
> The Power Automate cloud flows designer isn't yet available in integration surfaces such as Power Apps, Teams, and others.

:::image type="content" source="media/flows-designer/classic-designer.png" alt-text="Screenshot of the 'Switch to classic designer' button below the menu.":::

### See also

To learn more, go to [Get started with Copilot in cloud flows](get-started-with-copilot.md).


