# Salesforce DX Project: Next Steps

Now that you’ve created a Salesforce DX project, what’s next? Here are some documentation resources to get you started.

## What is the Component ?

Illustrations are great way to communicate the state of the component using svg instead of text only. You might see alot of illustrations from Salesforce standard components. This custom component leverages the SLDS for each illustration and provides a common component to render any of the illustration based on variant. It is further extended to add header or footer using slots.

##### How to use it?

```
<c-illustration
    size="large"
    variant="Going Camping"
    heading="Happy Learning!"
    message="Enjoy the ride!"
    show-footer
></c-illustration>
```

##### Component Parameters

| Name    | Default | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------- | ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| variant |         | The variant changes the type of illustration. Valid values are simply the names of the illustrations on the SLDS website.<br><br>[Going Camping](https://www.lightningdesignsystem.com/components/illustration/#Going-Camping)<br>[Maintenance](https://www.lightningdesignsystem.com/components/illustration/#Maintenance)<br>[Desert](https://www.lightningdesignsystem.com/components/illustration/#Desert)<br>[Open Road](https://www.lightningdesignsystem.com/components/illustration/#Open-Road)<br>[No Access](https://www.lightningdesignsystem.com/components/illustration/#No-Access)<br>[No Connection](https://www.lightningdesignsystem.com/components/illustration/#No-Connection)<br>[Not Available In Lightning](https://www.lightningdesignsystem.com/components/illustration/#Not-Available-In-Lightning)<br>[Page Not Available](https://www.lightningdesignsystem.com/components/illustration/#Page-Not-Available)<br>[Fishing Deals](https://www.lightningdesignsystem.com/components/illustration/#Fishing-Deals)<br>[Lake Mountain](https://www.lightningdesignsystem.com/components/illustration/#Lake-Mountain)<br>[No Events](https://www.lightningdesignsystem.com/components/illustration/#No-Events)<br>[No Task](https://www.lightningdesignsystem.com/components/illustration/#No-Task)<br>[Setup](https://www.lightningdesignsystem.com/components/illustration/#Setup)<br>[Gone Fishing](https://www.lightningdesignsystem.com/components/illustration/#Gone-Fishing)<br>[No Content](https://www.lightningdesignsystem.com/components/illustration/#No-Content)<br>[No Preview](https://www.lightningdesignsystem.com/components/illustration/#No-Preview)<br>[Research](https://www.lightningdesignsystem.com/components/illustration/#Research) |
| heading |         | The text to be shown as the heading                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| message |         | The text to be shown as the message                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| size    | small   | The size of the illustration. Valid values are small and large.<br>To make it responsive, declare the `@api flexipageRegionWidth;` variable in your component and pass it into this attribute like `size={flexipageRegionWidth}`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| show-footer    | false   | Adds footer to the illustration. You need to pass HTML to render as slot with name footer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

##### Slots

| Name                    | Description         | References                                                                                                                                                  |
| ----------------------- | -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Header | Use to add content to header of the illustration                  |    ```<p slot="header"> Todays Task <p>```                                                                                                                                                         |
| Footer              | Use to add content to the footer |```<lightning-button slot="footer" variant="base" name="Add Task"></lightning-button>```  |

## Deploy to Salesforce Org
https://githubsfdeploy.herokuapp.com/app/githubdeploy/kloudarts/lwc-illustration

## Read All About It

- [Salesforce Illustrations SLDS](https://www.lightningdesignsystem.com/components/illustration/)

