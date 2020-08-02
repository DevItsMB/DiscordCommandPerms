# DiscordCommandPerms



```java
bot.on('message', message => {
    // If the message is "$admin"
    if (message.content === '$admin') {

        const embed = new MessageEmbed()
        .setTitle('SRDR Donkk Track')  
        .setURL('https://steamcommunity.com/sharedfiles/filedetails/?id=2173283456')
        .setColor('#ffc90e')
        .setThumbnail('https://file.coffee/u/I137hILuT.png')
        .addFields(
            { name: 'Description', value: 'This is an easy track around the isle of donkk, the track is around the main highway counting with a tunnel and up hill climbs.' },
            { name: 'Spawn', value: 'You can spawn your car at the hangar' },
            /// { name: '\u200B', value: '\u200B' },
        )
        .setImage('https://media.discordapp.net/attachments/735113327084175410/735113861648089129/unknown.png?width=681&height=703')
        .setTimestamp()
        .setFooter('SRDR Bot © 2020');
      
          if (message.member.hasPermission("ADMINISTRATOR")) {
            message.channel.send(embed)
          } else {
            message.channel.send('Sorry, you cant use that command, If you believe this is an error contact an Admin')
          }
        };
})```
