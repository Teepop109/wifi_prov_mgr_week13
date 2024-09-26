rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:7176
load:0x40078000,len:15564
ho 0 tail 12 room 4
load:0x40080400,len:4
--- 0x40080400: _init at ??:?

load:0x40080404,len:3904
entry 0x40080640
I (31) boot: ESP-IDF v5.3.1 2nd stage bootloader
I (31) boot: compile time Sep 26 2024 13:38:44
I (31) boot: Multicore bootloader
I (35) boot: chip revision: v3.0
I (39) boot.esp32: SPI Speed      : 40MHz
I (44) boot.esp32: SPI Mode       : DIO
I (48) boot.esp32: SPI Flash Size : 2MB
I (53) boot: Enabling RNG early entropy source...
I (58) boot: Partition Table:
I (62) boot: ## Label            Usage          Type ST Offset   Length
I (69) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (77) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (84) boot:  2 factory          factory app      00 00 00010000 00140000
I (92) boot: End of partition table
I (96) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=2bb58h (179032) map
I (166) esp_image: segment 1: paddr=0003bb80 vaddr=3ffbdb60 size=04498h ( 17560) load
I (172) esp_image: segment 2: paddr=00040020 vaddr=400d0020 size=bba7ch (768636) map
I (436) esp_image: segment 3: paddr=000fbaa4 vaddr=3ffc1ff8 size=017a0h (  6048) load
I (438) esp_image: segment 4: paddr=000fd24c vaddr=40080000 size=1bfc0h (114624) load
I (501) boot: Loaded app from partition at offset 0x10000
I (501) boot: Disabling RNG early entropy source...
I (513) cpu_start: Multicore app
I (521) cpu_start: Pro cpu start user code
I (521) cpu_start: cpu freq: 160000000 Hz
I (522) app_init: Application information:
I (524) app_init: Project name:     wifi_prov_mgr
I (530) app_init: App version:      1
I (534) app_init: Compile time:     Sep 26 2024 13:38:07
I (540) app_init: ELF file SHA256:  e9ebeb99b...
I (545) app_init: ESP-IDF:          v5.3.1
I (550) efuse_init: Min chip rev:     v0.0
I (555) efuse_init: Max chip rev:     v3.99 
I (560) efuse_init: Chip rev:         v3.0
I (565) heap_init: Initializing. RAM available for dynamic allocation:
I (572) heap_init: At 3FFAFF10 len 000000F0 (0 KiB): DRAM
I (578) heap_init: At 3FFB6388 len 00001C78 (7 KiB): DRAM
I (584) heap_init: At 3FFB9A20 len 00004108 (16 KiB): DRAM
I (590) heap_init: At 3FFC9F90 len 00016070 (88 KiB): DRAM
I (596) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (603) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (609) heap_init: At 4009BFC0 len 00004040 (16 KiB): IRAM
I (617) spi_flash: detected chip: generic
I (620) spi_flash: flash io: dio
W (624) spi_flash: Detected size(4096k) larger than the size in the binary image header(2048k). Using the size in the binary image header.
I (638) coexist: coex firmware version: 4482466
I (643) main_task: Started on CPU0
I (653) main_task: Calling app_main()
I (693) wifi:wifi driver task: 3ffcdf04, prio:23, stack:6656, core=0
I (703) wifi:wifi firmware version: ccaebfa
I (703) wifi:wifi certification version: v7.0
I (703) wifi:config NVS flash: enabled
I (703) wifi:config nano formating: disabled
I (713) wifi:Init data frame dynamic rx buffer num: 32
I (713) wifi:Init static rx mgmt buffer num: 5
I (723) wifi:Init management short buffer num: 32
I (723) wifi:Init dynamic tx buffer num: 32
I (723) wifi:Init static rx buffer size: 1600
I (733) wifi:Init static rx buffer num: 10
I (733) wifi:Init dynamic rx buffer num: 32
I (743) wifi_init: rx ba win: 6
I (743) wifi_init: accept mbox: 6
I (743) wifi_init: tcpip mbox: 32
I (753) wifi_init: udp mbox: 6
I (753) wifi_init: tcp mbox: 6
I (763) wifi_init: tcp tx win: 5760
I (763) wifi_init: tcp rx win: 5760
I (763) wifi_init: tcp mss: 1440
I (773) wifi_init: WiFi IRAM OP enabled
I (773) wifi_init: WiFi RX IRAM OP enabled
I (783) wifi_prov_scheme_ble: BT memory released
I (783) app: Already provisioned, starting Wi-Fi STA
I (793) wifi_prov_scheme_ble: BTDM memory released
I (803) phy_init: phy_version 4830,54550f7,Jun 20 2024,14:22:08
I (873) wifi:mode : sta (94:b5:55:f2:65:8c)
I (873) wifi:enable tsf
I (3293) wifi:new:<11,0>, old:<1,0>, ap:<255,255>, sta:<11,0>, prof:1, snd_ch_cfg:0x0
I (3303) wifi:state: init -> auth (0xb0)
I (3313) wifi:state: auth -> assoc (0x0)
I (3323) wifi:state: assoc -> run (0x10)
I (3333) wifi:connected with AIS 4G Hi-Speed Home WiFi_769475, aid = 6, channel 11, BW20, bssid = 30:0a:c5:9e:94:9f
I (3333) wifi:security: WPA2-PSK, phy: bgn, rssi: -58
I (3343) wifi:pm start, type: 1

I (3343) wifi:dp: 1, bi: 102400, li: 3, scale listen interval from 307200 us to 307200 us
I (3403) wifi:AP's beacon interval = 102400 us, DTIM period = 1
I (4353) app: Connected with IP Address:192.168.1.155
I (4353) esp_netif_handlers: sta ip: 192.168.1.155, mask: 255.255.255.0, gw: 192.168.1.1
I (4353) app: Hello World!
I (5363) app: Hello World!
I (6363) app: Hello World!
I (6673) wifi:<ba-add>idx:0 (ifx:0, 30:0a:c5:9e:94:9f), tid:0, ssn:4, winSize:64
I (7363) app: Hello World!
I (8363) app: Hello World!
I (9363) app: Hello World!
ets Jul 29 2019 12:21:46

rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:7176
load:0x40078000,len:15564
ho 0 tail 12 room 4
load:0x40080400,len:4
--- 0x40080400: _init at ??:?

load:0x40080404,len:3904
entry 0x40080640
I (31) boot: ESP-IDF v5.3.1 2nd stage bootloader
I (31) boot: compile time Sep 26 2024 13:38:44
I (31) boot: Multicore bootloader
I (35) boot: chip revision: v3.0
I (39) boot.esp32: SPI Speed      : 40MHz
I (44) boot.esp32: SPI Mode       : DIO
I (48) boot.esp32: SPI Flash Size : 2MB
I (53) boot: Enabling RNG early entropy source...
I (58) boot: Partition Table:
I (62) boot: ## Label            Usage          Type ST Offset   Length
I (69) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (77) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (84) boot:  2 factory          factory app      00 00 00010000 00140000
I (92) boot: End of partition table
I (96) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=2bb58h (179032) map
I (166) esp_image: segment 1: paddr=0003bb80 vaddr=3ffbdb60 size=04498h ( 17560) load
I (172) esp_image: segment 2: paddr=00040020 vaddr=400d0020 size=bba7ch (768636) map
I (436) esp_image: segment 3: paddr=000fbaa4 vaddr=3ffc1ff8 size=017a0h (  6048) load
I (438) esp_image: segment 4: paddr=000fd24c vaddr=40080000 size=1bfc0h (114624) load
I (501) boot: Loaded app from partition at offset 0x10000
I (501) boot: Disabling RNG early entropy source...
I (513) cpu_start: Multicore app
I (521) cpu_start: Pro cpu start user code
I (521) cpu_start: cpu freq: 160000000 Hz
I (522) app_init: Application information:
I (524) app_init: Project name:     wifi_prov_mgr
I (530) app_init: App version:      1
I (534) app_init: Compile time:     Sep 26 2024 13:38:07
I (540) app_init: ELF file SHA256:  e9ebeb99b...
I (545) app_init: ESP-IDF:          v5.3.1
I (550) efuse_init: Min chip rev:     v0.0
I (555) efuse_init: Max chip rev:     v3.99
I (560) efuse_init: Chip rev:         v3.0
I (565) heap_init: Initializing. RAM available for dynamic allocation:
I (572) heap_init: At 3FFAFF10 len 000000F0 (0 KiB): DRAM
I (578) heap_init: At 3FFB6388 len 00001C78 (7 KiB): DRAM
I (584) heap_init: At 3FFB9A20 len 00004108 (16 KiB): DRAM
I (590) heap_init: At 3FFC9F90 len 00016070 (88 KiB): DRAM
I (596) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (603) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (609) heap_init: At 4009BFC0 len 00004040 (16 KiB): IRAM
I (617) spi_flash: detected chip: generic
I (620) spi_flash: flash io: dio
W (624) spi_flash: Detected size(4096k) larger than the size in the binary image header(2048k). Using the size in the binary image header.
I (638) coexist: coex firmware version: 4482466
I (643) main_task: Started on CPU0
I (653) main_task: Calling app_main()
I (693) wifi:wifi driver task: 3ffcdf04, prio:23, stack:6656, core=0
I (703) wifi:wifi firmware version: ccaebfa
I (703) wifi:wifi certification version: v7.0
I (703) wifi:config NVS flash: enabled
I (703) wifi:config nano formating: disabled
I (713) wifi:Init data frame dynamic rx buffer num: 32
I (713) wifi:Init static rx mgmt buffer num: 5
I (723) wifi:Init management short buffer num: 32
I (723) wifi:Init dynamic tx buffer num: 32
I (723) wifi:Init static rx buffer size: 1600
I (733) wifi:Init static rx buffer num: 10
I (733) wifi:Init dynamic rx buffer num: 32
I (743) wifi_init: rx ba win: 6
I (743) wifi_init: accept mbox: 6
I (743) wifi_init: tcpip mbox: 32
I (753) wifi_init: udp mbox: 6
I (753) wifi_init: tcp mbox: 6
I (763) wifi_init: tcp tx win: 5760
I (763) wifi_init: tcp rx win: 5760
I (763) wifi_init: tcp mss: 1440
I (773) wifi_init: WiFi IRAM OP enabled
I (773) wifi_init: WiFi RX IRAM OP enabled
I (783) wifi_prov_scheme_ble: BT memory released
I (883) app: Button pressed
I (883) app: Starting provisioning
I (883) app: Development mode: using hard coded salt
I (893) app: Development mode: using hard coded verifier
I (893) phy_init: phy_version 4830,54550f7,Jun 20 2024,14:22:08
I (973) wifi:mode : sta (94:b5:55:f2:65:8c)
I (973) wifi:enable tsf
I (983) BTDM_INIT: BT controller compile version [b022216]
I (983) BTDM_INIT: Bluetooth MAC: 94:b5:55:f2:65:8e
I (1223) protocomm_nimble: BLE Host Task Started
I (1233) wifi_prov_mgr: Provisioning started with service name : PROV_F2658C 
I (1243) app: Provisioning started
I (1243) app: Scan this QR code from the provisioning application for Provisioning.
I (1253) QRCODE: Encoding below text with ECC LVL 0 & QR Code Version 10
I (1253) QRCODE: {"ver":"v1","name":"PROV_F2658C","username":"wifiprov","pop":"abcd1234","transport":"ble"}
I (1283) NimBLE: GAP procedure initiated: advertise;
I (1283) NimBLE: disc_mode=2
I (1283) NimBLE:  adv_channel_map=0 own_addr_type=0 adv_filter_policy=0 adv_itvl_min=256 adv_itvl_max=256
I (1293) NimBLE:


  █▀▀▀▀▀█ ███ ▀▄▀▀▀▄▄▄█▄▀▀▄▄▀▀  █▀▀▀▀▀█
  █ ███ █ █▄▀█ ▄▄▄█▀▀▀▄▀▀█▄▄ ▄█ █ ███ █   
  █ ▀▀▀ █ ▄  ▄▄█▀▀▀  ▄▀█▄▀ ▀█▀▄ █ ▀▀▀ █
  ▀▀▀▀▀▀▀ ▀▄▀ █ █ █▄▀ ▀▄▀▄▀ ▀ █ ▀▀▀▀▀▀▀   
  █▀▄▄█▀▀   ▄▀▄▄█▄ ▀█▀▄▀██▀▄  ▄▄ █▄▀▀▀▀
  █▄▄▀█ ▀ █ ██▀▀ ▀█▄  ▄▄▄▀▄ █████ ▀█▄█▄   
   ▀██▄▄▀█ ▀▀ ▀  █▀██▀▀▀ ▄▀▄ █▀ ▀█▄▀█▄▀
   ▄▄█▀▀▀ ▀▄  ▄ █▀██▀▄▀▄██▀▀▄█ █▄█ █▄     
  ▀▀▄▄▄█▀▄▀▄▀▀▄▀█▄ ▀█▀▀█ █▀▄▄▄▀██▀▄ ▀▀▀   
   ▄ ▄ █▀  █▄█▀█▀█▀▄ ▄ █▄▀█ █▀▀█ █▄▀▄▄▄
  ▀▀ ▄▀▄▀▀▄▄█ ▀█▄▄█▀ ▀▀▀ ▄ ▄ ▄▀██▀▄█▀█▀   
  ▄█▄██▀▀   ▀ ▄ ▄▀██▀ ▀▄█▀ ▀ ▀██▄▀ █▄▄▄
  █▄ █▄ ▀▀ █▀▀▄▀▀▄█▀ ▀▀▀█▄█ ▄▄▀▀█▀▄▀▀ ▀   
    █▄▀▀▀▀▀▄▀█▀█▀▀ ▄ ▄ ██▀ ▀▀▀▀ █▄█▄█▀▄   
  ▀▀▀▀ ▀▀▀▄█▀ ▀█▄█▄▀▄▀██▀█▄▄▄ █▀▀▀█ ▀▄
  █▀▀▀▀▀█ ▄ █ ▄ ▄███▄▄ ▄ ▀  ▄▀█ ▀ ██▄▄▄   
  █ ███ █ ▀▄ ▀▄▀▀▄██▄ ▄▀█▄█ ▄▄████▀▄█▄▄
  █ ▀▀▀ █ ▄▄██▀█▀▀▄▄▀▄ ████ █ ▄  ▀▄██▄    
  ▀▀▀▀▀▀▀ ▀▀  ▀▀  ▀▀ ▀▀▀  ▀  ▀   ▀▀ ▀▀▀


I (1563) app: If QR code is not visible, copy paste the below URL in a browser.
https://espressif.github.io/esp-jumpstart/qrcode.html?data={"ver":"v1","name":"PROV_F2658C","username":"wifiprov","pop":"abcd1234","transport":"ble"}
I (12183) app: BLE transport: Connected!
I (12363) protocomm_nimble: mtu update event; conn_handle=0 cid=4 mtu=256
I (13083) security2: Using salt and verifier to generate public key...
I (13713) app: Secured session established!
W (116863) wifi:Password length matches WPA2 standards, authmode threshold changes from OPEN to WPA2
I (116903) app: Received Wi-Fi credentials
        SSID     : AIS 4G Hi-Speed Home WiFi_76947550769475
        Password : 50769475
I (123003) wifi:new:<11,0>, old:<1,0>, ap:<255,255>, sta:<11,0>, prof:1, snd_ch_cfg:0x0
I (123013) wifi:state: init -> auth (0xb0)
I (123023) wifi:state: auth -> assoc (0x0)
I (123033) wifi:state: assoc -> run (0x10)
I (123053) wifi:connected with AIS 4G Hi-Speed Home WiFi_769475, aid = 6, channel 11, BW20, bssid = 30:0a:c5:9e:94:9f
I (123053) wifi:security: WPA2-PSK, phy: bgn, rssi: -46
I (123073) wifi:pm start, type: 1

I (123073) wifi:dp: 1, bi: 102400, li: 3, scale listen interval from 307200 us to 307200 us
I (123073) wifi:AP's beacon interval = 102400 us, DTIM period = 1
I (124083) app: Connected with IP Address:192.168.1.155
I (124083) esp_netif_handlers: sta ip: 192.168.1.155, mask: 255.255.255.0, gw: 192.168.1.1
I (124083) wifi_prov_mgr: STA Got IP
I (124093) app: Provisioning successful
I (124093) app: Hello World!
I (125093) app: Hello World!
I (126093) app: Hello World!
I (127093) app: Hello World!
I (128093) app: Hello World!
I (128243) NimBLE: GAP procedure initiated: stop advertising.

I (128243) NimBLE: GAP procedure initiated: stop advertising.

I (128253) NimBLE: GAP procedure initiated: terminate connection; conn_handle=0 hci_reason=19

E (128313) protocomm_nimble: Error setting advertisement data; rc = 30
I (128323) wifi_prov_mgr: Provisioning stopped
I (128333) app: BLE transport: Disconnected!
I (128333) wifi_prov_scheme_ble: BTDM memory released
I (129093) app: Hello World!
I (130093) app: Hello World!
I (130953) wifi:<ba-add>idx:0 (ifx:0, 30:0a:c5:9e:94:9f), tid:0, ssn:4, winSize:64
I (131093) app: Hello World!
I (132093) app: Hello World!
I (133093) app: Hello World!
I (134093) app: Hello World!
I (135093) app: Hello World!
I (136093) app: Hello World!
