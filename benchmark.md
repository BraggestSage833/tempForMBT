## Minecraft load time benchmark


---

<p align="center" style="font-size:160%;">
MC total load time:<br>
206.43 sec
<br>
<sup><sub>(
3:26 min
)</sub></sup>
</p>

<br>


<p align="center">
<img src="https://quickchart.io/chart?w=400&h=30&c={%20type:%20'horizontalBar',%20data:%20{%20datasets:%20[%20{label:%20'MODS:',%20data:%20[104.69]},%20{label:%20'FML%20stuff:',%20data:%20[101.74]}%20]%20},%20options:%20{%20scales:%20{%20xAxes:%20[{display:%20false,stacked:%20true}],%20yAxes:%20[{display:%20false,stacked:%20true}],%20},%20elements:%20{rectangle:%20{borderWidth:%202}},%20legend:%20{display:%20false,},%20plugins:%20{datalabels:%20{color:%20'white',formatter:%20(value,%20context)%20=>%20[context.dataset.label,%20value].join('%20')%20}}%20}%20}"/>
</p>

<br>

# Mods Loading Time
<p align="center">
<img src="https://quickchart.io/chart?w=400&h=300&c={%20type:%20'outlabeledPie',%20options:%20{%20cutoutPercentage:%2025,%20plugins:%20{%20legend:%20!1,%20outlabels:%20{%20stretch:%205,%20padding:%201,%20text:%20(v,i)=>[%20v.labels[v.dataIndex],'%20',%20(v.percent*1000|0)/10,%20String.fromCharCode(37)].join('')%20}%20}%20},%20data:%20{...%20`%20436e17%2025.03s%20Had%20Enough%20Items;%20214d9e%209.02s%20Minecraft%20Forge;%20516fa8%207.80s%20Ender%20IO;%208f304e%206.42s%20Astral%20Sorcery;%208f3087%203.54s%20Forge%20Mod%20Loader;%205161a8%202.36s%20CraftTweaker2;%20495797%200.88s%20CraftTweaker2%20(Script%20Loading);%20382c5a%202.72s%20GregTech%20Community%20Edition;%20cd2c34%202.59s%20Hooked;%208451a8%202.45s%20LibrarianLib%20Stage%202;%20cd2c77%202.39s%20Logistics%20Pipes;%203e68ba%202.07s%20AE2%20Unofficial%20Extended%20Life;%203e6cba%202.01s%20Random%20Things;%206e173f%201.97s%20Gregicality;%208f308f%201.94s%20JourneyMap;%20ba6a3e%201.46s%20Advanced%20Rocketry;%20cd872c%201.28s%20LittleTiles;%202d176e%201.08s%20Ender%20IO%20Machines;%205a352c%201.05s%20Shadowfacts'%20Forgelin;%2095219e%200.92s%20ContentTweaker;%20642151%200.91s%20BD%20Lib;%20444444%200.00s%200%20Other%20mods;%20333333%2023.97s%2069%20'Fast'%20mods%20(load%201.0s%20-%200.1s);%20222222%202.66s%2079%20'Instant'%20mods%20(load%20%3C%200.1s)%20`%20.split(';').reduce((a,%20l)%20=>%20{%20l.match(/(\w{6})%20*(\d*\.\d*)s%20(.*)/)%20.slice(1).map((a,%20i)%20=>%20[[String.fromCharCode(35),a].join(''),%20parseFloat(a),%20a][i])%20.forEach((s,%20i)%20=>%20[a.datasets[0].backgroundColor,%20a.datasets[0].data,%20a.labels][i].push(s)%20);%20return%20a%20},%20{%20labels:%20[],%20datasets:%20[{%20backgroundColor:%20[],%20data:%20[],%20borderColor:%20'rgba(22,22,22,0.3)',%20borderWidth:%201%20}]%20})%20}%20}"/>
</p>

<br>

# Top Mods Details (except JEI, FML and Forge)
<p align="center">
<img src="https://quickchart.io/chart?w=400&h=450&c={%20options:%20{%20scales:%20{%20xAxes:%20[{stacked:%20true}],%20yAxes:%20[{stacked:%20true}],%20},%20plugins:%20{%20datalabels:%20{%20anchor:%20'end',%20align:%20'top',%20color:%20'white',%20backgroundColor:%20'rgba(46,%20140,%20171,%200.6)',%20borderColor:%20'rgba(41,%20168,%20194,%201.0)',%20borderWidth:%200.5,%20borderRadius:%203,%20padding:%200,%20font:%20{size:10},%20formatter:%20(v,ctx)%20=>%20ctx.datasetIndex!=ctx.chart.data.datasets.length-1%20?%20null%20:%20[((ctx.chart.data.datasets.reduce((a,b)=>a-%20-b.data[ctx.dataIndex],0)*10)|0)/10,'s'].join('')%20},%20colorschemes:%20{%20scheme:%20'office.Damask6'%20}%20}%20},%20type:%20'bar',%20data:%20{...(()%20=>%20{%20let%20a%20=%20{%20labels:%20[],%20datasets:%20[]%20};%20`%201:%20Construction;%202:%20Loading%20Resources;%203:%20PreInitialization;%204:%20Initialization;%205:%20InterModComms$IMC;%206:%20PostInitialization;%207:%20LoadComplete;%208:%20ModIdMapping%20`%20.split(';')%20.map(l%20=>%20l.match(/\d:%20(.*)/).slice(1))%20.forEach(([name])%20=>%20a.datasets.push({%20label:%20name,%20data:%20[]%20}));%20`%201%202%203%204%205%206%207%208%20;%20Had%20Enough%20Items%20|%200.07|%200.00|%200.48|%200.01|%200.00|%200.00|%2024.46|%200.00;%20Ender%20IO%20|%202.38|%200.00|%202.98|%200.26|%202.06|%200.07|%200.00|%200.05;%20Astral%20Sorcery%20|%200.19|%200.00|%204.92|%200.73|%200.00|%200.58|%200.00|%200.00;%20CraftTweaker2%20|%200.60|%200.00|%201.82|%200.00|%200.00|%200.83|%200.00|%200.00;%20GregTech%20Community%20Edition%20|%200.17|%200.01|%201.52|%200.62|%200.00|%200.41|%200.00|%200.00;%20Hooked%20|%200.10|%200.00|%202.49|%200.00|%200.00|%200.00|%200.00|%200.00;%20LibrarianLib%20Stage%202%20|%200.01|%200.03|%202.39|%200.02|%200.00|%200.01|%200.00|%200.00;%20Logistics%20Pipes%20|%200.55|%200.00|%201.40|%200.25|%200.00|%200.19|%200.00|%200.00;%20AE2%20Unofficial%20Extended%20Life%20|%200.16|%200.01|%201.37|%200.13|%200.10|%200.31|%200.00|%200.00;%20Random%20Things%20|%200.13|%200.00|%201.61|%200.08|%200.00|%200.19|%200.00|%200.00;%20Gregicality%20|%200.46|%200.00|%201.45|%200.06|%200.00|%200.00|%200.00|%200.00;%20JourneyMap%20|%200.04|%200.01|%200.03|%200.77|%200.00|%201.09|%200.00|%200.00%20`%20.split(';').slice(1)%20.map(l%20=>%20l.split('|').map(s%20=>%20s.trim()))%20.forEach(([name,%20...arr],%20i)%20=>%20{%20a.labels.push(name);%20arr.forEach((v,%20j)%20=>%20a.datasets[j].data[i]%20=%20v)%20});%20return%20a%20})()}%20}"/>
</p>

<br>

# TOP JEI Registered Plugis
<p align="center">
<img src="https://quickchart.io/chart?w=700&c={%20options:%20{%20elements:%20{%20rectangle:%20{%20borderWidth:%201%20}%20},%20legend:%20false%20},%20type:%20'horizontalBar',%20data:%20{...(()%20=>%20{%20let%20a%20=%20{%20labels:%20[],%20datasets:%20[{%20backgroundColor:%20'rgba(0,%2099,%20132,%200.5)',%20borderColor:%20'rgb(0,%2099,%20132)',%20data:%20[]%20}]%20};%20`%201.76:%20crazypants.enderio.machines.integration.jei.MachinesPlugin;%201.35:%20gregicadditions.jei.JEIGAPlugin;%200.72:%20mezz.jei.plugins.vanilla.VanillaPlugin;%200.17:%20crazypants.enderio.base.integration.jei.JeiPlugin;%200.14:%20gregtech.integration.jei.GTJeiPlugin;%200.09:%20hellfirepvp.astralsorcery.common.integrations.ModIntegrationJEI;%200.06:%20zmaster587.advancedRocketry.integration.jei.ARPlugin;%200.05:%20com.brandon3055.draconicevolution.integration.jei.DEJEIPlugin;%200.04:%20de.ellpeck.actuallyadditions.mod.jei.JEIActuallyAdditionsPlugin;%200.04:%20appeng.integration.modules.jei.JEIPlugin;%200.03:%20crafttweaker.mods.jei.JEIAddonPlugin;%200.03:%20lumien.randomthings.handler.compability.jei.RandomThingsPlugin;%200.03:%20eutros.multiblocktweaker.jei.MultiblockTweakerJEIPlugin;%200.02:%20logisticspipes.modplugins.jei.JEIPluginLoader;%200.02:%20fi.dy.masa.enderutilities.compat.jei.EnderUtilitiesJeiPlugin;%200.22:%20Other%2041%20Plugins%20`%20.split(';')%20.map(l%20=>%20l.split(':'))%20.forEach(([time,%20name])%20=>%20{%20a.labels.push(name);%20a.datasets[0].data.push(time)%20})%20;%20return%20a%20})()%20}%20}"/>
</p>

<br>

# FML Stuff
<p align="center">
<img src="https://quickchart.io/chart?w=500&h=400&c={%20options:%20{%20rotation:%20Math.PI,%20cutoutPercentage:%2055,%20plugins:%20{%20legend:%20!1,%20outlabels:%20{%20stretch:%205,%20padding:%201,%20text:%20(v)=>v.labels%20},%20doughnutlabel:%20{%20labels:%20[%20{%20text:%20'FML%20stuff:',%20color:%20'rgba(128,%20128,%20128,%200.5)',%20font:%20{size:%2018}%20},%20{%20text:%20[101.74,'s'].join(''),%20color:%20'rgba(128,%20128,%20128,%201)',%20font:%20{size:%2022}%20}%20]%20},%20}%20},%20type:%20'outlabeledPie',%20data:%20{...(()%20=>%20{%20let%20a%20=%20{%20labels:%20[],%20datasets:%20[{%20backgroundColor:%20[],%20data:%20[],%20borderColor:%20'rgba(22,22,22,0.3)',%20borderWidth:%202%20}]%20};%20`%20993A00%209.18s%20Loading%20sounds;%20994400%209.24s%20Loading%20Resource%20-%20SoundHandler;%20994F00%2026.84s%20ModelLoader:%20blocks;%20995900%206.70s%20ModelLoader:%20items;%20996300%203.26s%20ModelLoader:%20baking;%20996D00%200.11s%20Applying%20remove%20recipe%20actions;%20997700%200.16s%20Applying%20remove%20furnace%20recipe%20actions;%20444444%2046.26s%20Other%20`%20.split(';')%20.map(l%20=>%20l.match(/(\w{6})%20*(\d*\.\d*)s%20(.*)/))%20.forEach(([,%20col,%20time,%20name])%20=>%20{%20a.labels.push([name,%20'%20',%20time,%20's'].join(''));%20a.datasets[0].data.push(parseFloat(time));%20a.datasets[0].backgroundColor.push([String.fromCharCode(35),%20col].join(''))%20})%20;%20return%20a%20})()}%20}"/>
</p>

<br>
