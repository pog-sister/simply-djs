# ticketSystem function
#### This is an example of ticketSystem (discord-buttons required)
<br>

## With Customization
```js
const simplydjs = require('simply-djs')

client.on('clickButton', async(button) => { 
    // a discord-buttons event which fires when a button gets clicked
simplydjs.clickBtn(button, {
    embedDesc: 'embed description',
    embedColor: 'hex code', // default: #075FFF
    closeColor: 'color from buttons', //default: blurple
    closeEmoji: 'emoji id', // default: 🔒
    delColor: 'color from buttons', // default: grey
    delEmoji: 'emoji id', // default: ❌
    openColor: 'color from buttons' , // default: green
    openEmoji: 'emoji id' // default: 🔓
    })
})

// message event
// setup-ticket command

simplydjs.ticketSystem(message, message.channel, {
     embedDesc: 'embed description', // default: '🎫 Create a ticket by clicking the button 🎫'
    embedColor: 'hex code', // default: #075FFFF
    embedFoot: 'footer text', // default: message.guild.name
    emoji: 'emoji id', // default: 🎫
    color: 'color from buttons' // default: blurple
})
```
## Without Customization
```js
const simplydjs = require('simply-djs')

client.on('clickButton', async(button) => { 
    // a discord-buttons event which fires when a button gets clicked
simplydjs.clickBtn(button)
})

// message event
// setup-ticket command

simplydjs.ticketSystem(message, message.channel)
```

# Options for clickBtn function (Optional)
### Embed
- **embedDesc:** The Embed Description of the embed which is sent when the ticket has been opened
- **embedColor:** The Embed Color of the embed which is sent when the ticket has been opened

### Close Ticket Button
- **closeColor:** The color of the Close Ticket Button (Only red, green, grey/gray, blurple allowed)
- **closeEmoji:** The emoji for the Close Ticket Button (Only Emoji ID)

### Delete Ticket Button
- **delColor:** The color of the Delete Ticket Button (Only red, green, grey/gray, blurple allowed)
- **delEmoji:** The emoji for the Delete Ticket Button (Only Emoji ID)

### Reopen Ticket Button
- **openColor:** The color of the Delete Ticket Button (Only red, green, grey/gray, blurple allowed)
- **openEmoji:** The emoji for the Delete Ticket Button (Only Emoji ID)

# Options for ticketSystem function (Optional)
### Embed
- **embedDesc:** The Description for the Ticket System Embed (Embed that has ticket button that opens a ticket)
- **embedColor:** The Color of the Ticket System Embed (Embed that has ticket button that opens a ticket)
- **embedFoot:** The Footer for the Ticket System Embed (Embed that has ticket button that opens a ticket)

### Buttons
- **emoji:** The Emoji for the Ticket Button which opens a ticket (Only Emoji ID)
- **color:** The Color for the Ticket Button which opens a ticket. (Only red, green, grey/gray, blurple allowed)