So i am a nitwit
i thought i had all my dependencies install but i didnt

---- Minecraft Crash Report ----
// Shall we play a game?

Time: 2026-02-27 21:50:01
Description: Mod loading error has occurred

java.lang.Exception: Mod Loading has failed
	at TRANSFORMER/net.minecraftforge.forge@61.0.10/net.minecraftforge.logging.CrashReportExtender.dumpModLoadingCrashReport(CrashReportExtender.java:49) ~[forge-1.21.11-61.0.10-universal.jar:?]
	at TRANSFORMER/net.minecraftforge.forge@61.0.10/net.minecraftforge.client.loading.ClientModLoader.completeModLoading(ClientModLoader.java:112) ~[forge-1.21.11-61.0.10-universal.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.lambda$new$7(Minecraft.java:666) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.util.Util.ifElse(Util.java:636) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.lambda$new$8(Minecraft.java:659) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.gui.screens.LoadingOverlay.tick(LoadingOverlay.java:137) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.tick(Minecraft.java:1821) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.runTick(Minecraft.java:1273) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.run(Minecraft.java:893) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.main.Main.main(Main.java:223) ~[forge-1.21.11-61.0.10-client.jar:?]
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?]
	at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?]
	at SECURE-BOOTSTRAP/net.minecraftforge.fmlloader@1.21.11-61.0.10/net.minecraftforge.fml.loading.targets.CommonLaunchHandler.runTarget(CommonLaunchHandler.java:96) ~[fmlloader-1.21.11-61.0.10.jar!/:?]
	at SECURE-BOOTSTRAP/net.minecraftforge.fmlloader@1.21.11-61.0.10/net.minecraftforge.fml.loading.targets.CommonLaunchHandler.lambda$makeService$0(CommonLaunchHandler.java:79) ~[fmlloader-1.21.11-61.0.10.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:77) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:97) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.Launcher.run(Launcher.java:116) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.Launcher.main(Launcher.java:75) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.BootstrapEntry.main(BootstrapEntry.java:17) [modlauncher-10.2.4.jar!/:?]
	at net.minecraftforge.bootstrap@2.1.7/net.minecraftforge.bootstrap.Bootstrap.moduleMain(Bootstrap.java:188) [bootstrap-2.1.8.jar!/:?]
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?]
	at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?]
	at net.minecraftforge.bootstrap.Bootstrap.bootstrapMain(Bootstrap.java:133) [bootstrap-2.1.8.jar:2.1.8]
	at net.minecraftforge.bootstrap.Bootstrap.start(Bootstrap.java:53) [bootstrap-2.1.8.jar:2.1.8]
	at net.minecraftforge.bootstrap.ForgeBootstrap.main(ForgeBootstrap.java:19) [bootstrap-2.1.8.jar:2.1.8]
Transformer Audit:
  net.minecraft.client.Minecraft
    REASON: classloading
    PLUGIN: accesstransformer:BEFORE
  net.minecraft.client.gui.screens.LoadingOverlay
    REASON: classloading
  net.minecraft.client.main.Main
    REASON: classloading
  net.minecraft.util.Util
    REASON: classloading
  net.minecraftforge.client.loading.ClientModLoader
    REASON: classloading
  net.minecraftforge.logging.CrashReportExtender
    REASON: classloading


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Suspected Mods: NONE
Stacktrace:
	at TRANSFORMER/net.minecraftforge.forge@61.0.10/net.minecraftforge.logging.CrashReportExtender.lambda$dumpModLoadingCrashReport$7(CrashReportExtender.java:52) ~[forge-1.21.11-61.0.10-universal.jar!/:?]
Transformer Audit:
  net.minecraftforge.logging.CrashReportExtender
    REASON: classloading
-- MOD biomeswevegone --
Details:
	Mod File: /C:/Users/i aint tellin you my name reddit/AppData/Roaming/.minecraft/mods/Oh-The-Biomes-Weve-Gone-Forge-4.3.1.jar
	Failure message: Mod biomeswevegone requires geckolib 5.4 or above
		Currently, geckolib is not installed
	Mod Version: 4.3.1
	Mod Issue URL: https://github.com/Potion-Studios/Oh-The-Biomes-Weve-Gone/issues
	Exception message: MISSING EXCEPTION MESSAGE
Stacktrace:
	at TRANSFORMER/net.minecraftforge.forge@61.0.10/net.minecraftforge.logging.CrashReportExtender.lambda$dumpModLoadingCrashReport$7(CrashReportExtender.java:52) ~[forge-1.21.11-61.0.10-universal.jar:?]
	at java.base/java.util.ArrayList.forEach(ArrayList.java:1596) ~[?:?]
	at TRANSFORMER/net.minecraftforge.forge@61.0.10/net.minecraftforge.logging.CrashReportExtender.dumpModLoadingCrashReport(CrashReportExtender.java:50) ~[forge-1.21.11-61.0.10-universal.jar:?]
	at TRANSFORMER/net.minecraftforge.forge@61.0.10/net.minecraftforge.client.loading.ClientModLoader.completeModLoading(ClientModLoader.java:112) ~[forge-1.21.11-61.0.10-universal.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.lambda$new$7(Minecraft.java:666) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.util.Util.ifElse(Util.java:636) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.lambda$new$8(Minecraft.java:659) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.gui.screens.LoadingOverlay.tick(LoadingOverlay.java:137) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.tick(Minecraft.java:1821) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.runTick(Minecraft.java:1273) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.Minecraft.run(Minecraft.java:893) ~[forge-1.21.11-61.0.10-client.jar:?]
	at TRANSFORMER/minecraft@1.21.11/net.minecraft.client.main.Main.main(Main.java:223) ~[forge-1.21.11-61.0.10-client.jar:?]
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?]
	at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?]
	at SECURE-BOOTSTRAP/net.minecraftforge.fmlloader@1.21.11-61.0.10/net.minecraftforge.fml.loading.targets.CommonLaunchHandler.runTarget(CommonLaunchHandler.java:96) ~[fmlloader-1.21.11-61.0.10.jar!/:?]
	at SECURE-BOOTSTRAP/net.minecraftforge.fmlloader@1.21.11-61.0.10/net.minecraftforge.fml.loading.targets.CommonLaunchHandler.lambda$makeService$0(CommonLaunchHandler.java:79) ~[fmlloader-1.21.11-61.0.10.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:77) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:97) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.Launcher.run(Launcher.java:116) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.Launcher.main(Launcher.java:75) [modlauncher-10.2.4.jar!/:?]
	at SECURE-BOOTSTRAP/cpw.mods.modlauncher@10.2.4/cpw.mods.modlauncher.BootstrapEntry.main(BootstrapEntry.java:17) [modlauncher-10.2.4.jar!/:?]
	at net.minecraftforge.bootstrap@2.1.7/net.minecraftforge.bootstrap.Bootstrap.moduleMain(Bootstrap.java:188) [bootstrap-2.1.8.jar!/:?]
	at java.base/jdk.internal.reflect.DirectMethodHandleAccessor.invoke(DirectMethodHandleAccessor.java:103) ~[?:?]
	at java.base/java.lang.reflect.Method.invoke(Method.java:580) ~[?:?]
	at net.minecraftforge.bootstrap.Bootstrap.bootstrapMain(Bootstrap.java:133) [bootstrap-2.1.8.jar:2.1.8]
	at net.minecraftforge.bootstrap.Bootstrap.start(Bootstrap.java:53) [bootstrap-2.1.8.jar:2.1.8]
	at net.minecraftforge.bootstrap.ForgeBootstrap.main(ForgeBootstrap.java:19) [bootstrap-2.1.8.jar:2.1.8]
Transformer Audit:
  net.minecraft.client.Minecraft
    REASON: classloading
    PLUGIN: accesstransformer:BEFORE
  net.minecraft.client.gui.screens.LoadingOverlay
    REASON: classloading
  net.minecraft.client.main.Main
    REASON: classloading
  net.minecraft.util.Util
    REASON: classloading
  net.minecraftforge.client.loading.ClientModLoader
    REASON: classloading
  net.minecraftforge.logging.CrashReportExtender
    REASON: classloading


-- MOD wormhole --
Details:
	Mod File: /C:/Users/i aint tellin you my name reddit/AppData/Roaming/.minecraft/mods/wormhole-1.1.16-forge-mc1.21.11.jar
	Failure message: Mod wormhole requires supermartijn642configlib 1.1.6 or above
		Currently, supermartijn642configlib is not installed
	Mod Version: 1.1.16
	Mod Issue URL: https://github.com/SuperMartijn642/Wormhole/issues
	Exception message: MISSING EXCEPTION MESSAGE

-- MOD seasonhud --
Details:
	Mod File: /C:/Users/i aint tellin you my name reddit/AppData/Roaming/.minecraft/mods/SeasonHud-forge-1.21.11-2.0.0.jar
	Failure message: Mod seasonhud requires forgeconfigapiport 20.4.1 or above
		Currently, forgeconfigapiport is not installed
	Mod Version: 2.0.0
	Mod Issue URL: https://github.com/IanMods/SeasonHUD/issues
	Exception message: MISSING EXCEPTION MESSAGE

-- MOD biomeswevegone --
Details:
	Mod File: /C:/Users/i aint tellin you my name reddit/AppData/Roaming/.minecraft/mods/Oh-The-Biomes-Weve-Gone-Forge-4.3.1.jar
	Failure message: Mod biomeswevegone requires corgilib 9.0.0.0 or above
		Currently, corgilib is not installed
	Mod Version: 4.3.1
	Mod Issue URL: https://github.com/Potion-Studios/Oh-The-Biomes-Weve-Gone/issues
	Exception message: MISSING EXCEPTION MESSAGE

-- MOD biomeswevegone --
Details:
	Mod File: /C:/Users/i aint tellin you my name reddit/AppData/Roaming/.minecraft/mods/Oh-The-Biomes-Weve-Gone-Forge-4.3.1.jar
	Failure message: Mod biomeswevegone requires ohthetreesyoullgrow 9.0.0 or above
		Currently, ohthetreesyoullgrow is not installed
	Mod Version: 4.3.1
	Mod Issue URL: https://github.com/Potion-Studios/Oh-The-Biomes-Weve-Gone/issues
	Exception message: MISSING EXCEPTION MESSAGE

-- MOD openpartiesandclaims --
Details:
	Mod File: /C:/Users/i aint tellin you my name reddit/AppData/Roaming/.minecraft/mods/open-parties-and-claims-forge-1.21.11-0.25.10.jar
	Failure message: Mod openpartiesandclaims requires forgeconfigapiport 21.11.1 or above
		Currently, forgeconfigapiport is not installed
	Mod Version: 0.25.10
	Mod Issue URL: https://github.com/thexaero/open-parties-and-claims/issues
	Exception message: MISSING EXCEPTION MESSAGE

-- System Details --
Details:
	Minecraft Version: 1.21.11
	Minecraft Version ID: 1.21.11
	Operating System: Windows 11 (amd64) version 10.0
	Java Version: 21.0.7, Microsoft
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Microsoft
	Memory: 206176016 bytes (196 MiB) / 603979776 bytes (576 MiB) up to 2147483648 bytes (2048 MiB)
	CPUs: 8
	Processor Vendor: GenuineIntel
	Processor Name: Intel(R) Core(TM) i5-8250U CPU @ 1.60GHz
	Identifier: Intel64 Family 6 Model 142 Stepping 10
	Microarchitecture: Coffee Lake
	Frequency (GHz): 1.80
	Number of physical packages: 1
	Number of physical CPUs: 4
	Number of logical CPUs: 8
	Graphics card #0 name: Intel(R) UHD Graphics 620
	Graphics card #0 vendor: Intel Corporation
	Graphics card #0 VRAM (MiB): 1024.00
	Graphics card #0 deviceId: VideoController1
	Graphics card #0 versionInfo: 25.20.100.6446
	Memory slot #0 capacity (MiB): 8192.00
	Memory slot #0 clockSpeed (GHz): 2.40
	Memory slot #0 type: DDR4
	Virtual memory max (MiB): 14682.16
	Virtual memory used (MiB): 9172.43
	Swap memory total (MiB): 6656.00
	Swap memory used (MiB): 382.11
	Space in storage for jna.tmpdir (MiB): available: 681731.81, total: 937206.00
	Space in storage for org.lwjgl.system.SharedLibraryExtractPath (MiB): available: 681731.81, total: 937206.00
	Space in storage for io.netty.native.workdir (MiB): available: 681731.81, total: 937206.00
	Space in storage for java.io.tmpdir (MiB): available: 681731.81, total: 937206.00
	Space in storage for workdir (MiB): available: 681731.81, total: 937206.00
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	Debug Flags: 0 total; 
	ModLauncher: 10.2.4
	ModLauncher launch target: forge_client
	ModLauncher naming: mcp
	ModLauncher services: 
		/ slf4jfixer PLUGINSERVICE 
		/ runtimedistcleaner PLUGINSERVICE 
		/ runtime_enum_extender PLUGINSERVICE 
		/ capability_token_subclass PLUGINSERVICE 
		/ accesstransformer PLUGINSERVICE 
		/ mixin PLUGINSERVICE 
		/ fml TRANSFORMATIONSERVICE 
		/ forge TRANSFORMATIONSERVICE 
		/ mixin TRANSFORMATIONSERVICE 
	FML Language Providers: 
		lowcodefml@61
		minecraft@1.0
		javafml@61.0.10
	Mod List: 
		forge-1.21.11-61.0.10-client.jar                  |Minecraft                     |minecraft                     |1.21.11             |NONE      |Manifest: NOSIGNATURE
		forge-1.21.11-61.0.10-universal.jar               |Forge                         |forge                         |61.0.10             |NONE      |Manifest: 84:CE:76:E8:45:35:E4:0E:63:86:DF:47:59:80:0F:67:6C:C1:5F:6E:5F:4D:B3:54:47:1A:9F:7F:ED:5E:F2:90
