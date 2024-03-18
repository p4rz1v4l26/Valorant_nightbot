# Chat-Valorant-Rank
This API lets you fetch your rank dynamically, typically for making **!rank** command in your Twitch/YouTube stream.

**This API is developed and maintained by @kyroskoh and you can check it out here 'https://community.nightdev.com/t/custom-api-valorant-mmr-rank-api-v1/30536'**<br>


### THIS IS AVAILABLE FOR ALL REGIONS

# StreamElements/NightBot Usage

Replace `region` with your account's region code, `name` with your Valorant username and `tag` with your hashtag.


## Region Codes

| Region Code | Corresponding Region |
| ----------- | -------------------- |
| ap          | Asia/Pacific         |
| br          | Brazil               |
| eu          | Europe               |
| kr          | Korea                |
| latam       | Latin America        |
| na          | North America        |


<hr>

# Commands for Nightbot
<hr>

## Rank only

1. If you want to display only Rank with RR<br>
 ``` bash
   !addcom !rank $(urlfetch https://api.kyroskoh.xyz/valorant/v1/mmr/region/username/tag)
 ```

2. If you want your name and tag to be shown then use: <br>
``` bash
   !addcom !rank $(urlfetch https://api.kyroskoh.xyz/valorant/v1/mmr/region/name/tag?show=combo&display=1)
   ```

3. If you want to display the ID, Tag, Region with rank, RR and Elo : <br> 
``` bash
   !addcom !rank $(urlfetch https://api.kyroskoh.xyz/valorant/v1/mmr/region/name/tag?show=all&display=1)
   ```

4. if you don't want to display ID Tag,but Region with showing rank, RR and Elo: <br> 
```bash
   !addcom !rank $(urlfetch https://api.kyroskoh.xyz/valorant/v1/mmr/region/name/tag?show=all&display=0)
   ```
   ### Make sure to replace region,name

<hr>

# Example

Here is an example for my account. This would work for most accounts.
+ Example 
  * Username: `P4RZ1V4L#2610`
  * Account Region: `Asia/Pacific`
  * URL: `$(urlfetch https://api.kyroskoh.xyz/valorant/v1/mmr/AP/P4RZ1V4L/2610)`


<hr>

## Other Commands

1. Last ranked match rank points changes: <br>
``` bash 
 !addcom !lastcomp $(urlfetch https://api.kyroskoh.xyz/valorant/v1/mmrchange/region/name/tag)
```
2. Last match Stats:<br>
```bash
!addcom !lastmatch $(urlfetch https://api.kyroskoh.xyz/valorant/v1/lastmatchstats/region/name/tag)
```
3. Win loss in last 24 Hrs.
```bash
!addcom !winlose $(urlfetch https://api.kyroskoh.xyz/valorant/v1/winlose/region/name/tag)
```

<hr>

## You can make custom combinations also 

e.g. 
* add 
``` bash
?show=all&display=1
```
 as a prefix it will show all details like name , tag and region .

 * add 
``` bash
?show=rronly&display=0
```
 as a prefix it will show only rank rating and hide other details. 

 and many more 
 <hr>

 ##### If you want to make a dynamic command for chat which allows chat to find their own info such as Rank , lastmatch , lastcomp and etc contact me i would love to help.

<hr>


## Contact Details

If you have any questions or inquiries, please feel free to get in touch:

- Email: avinash.warale@yandex.com
- Discord: [@p4rz1v4l26](https://discordapp.com/users/896411007797325824/)

or you can join 
- [Discord server](https://discord.gg/vFWB2KGcH9)

