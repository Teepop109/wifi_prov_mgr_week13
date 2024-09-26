PS C:\Users\RYZEN 5\ESP_32wifipro\wifi_prov_mgr> & set IDF_PATH='C:\Users\RYZEN 5\esp_new\v5.3.1\esp-idf'
PS C:\Users\RYZEN 5\ESP_32wifipro\wifi_prov_mgr> & 'c:\esp_project\esp_1\python_env\idf5.3_py3.11_env\Scripts\python.exe' 'C:\Users\RYZEN 5\esp_new\v5.3.1\esp-idf\tools\idf_monitor.py' -p COM3 -b 115200 --toolchain-prefix xtensa-esp32-elf- --target esp32 'c:\Users\RYZEN 5\ESP_32wifipro\wifi_prov_mgr\build\wifi_prov_mgr.elf'
--- Warning: GDB cannot open serial ports accessed as COMx
--- Using \\.\COM3 instead...
--- esp-idf-monitor 1.5.0 on \\.\COM3 115200
--- Quit: Ctrl+] | Menu: Ctrl+T | Help: Ctrl+T followed by Ctrl+H
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
I (96) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=2b8d8h (178392) map
I (165) esp_image: segment 1: paddr=0003b900 vaddr=3ffbdb60 size=04718h ( 18200) load
I (172) esp_image: segment 2: paddr=00040020 vaddr=400d0020 size=bb524h (767268) map
I (436) esp_image: segment 3: paddr=000fb54c vaddr=3ffc2278 size=014c8h (  5320) load
I (438) esp_image: segment 4: paddr=000fca1c vaddr=40080000 size=1bfc0h (114624) load
I (500) boot: Loaded app from partition at offset 0x10000
I (501) boot: Disabling RNG early entropy source...
I (513) cpu_start: Multicore app
I (521) cpu_start: Pro cpu start user code
I (521) cpu_start: cpu freq: 160000000 Hz
I (521) app_init: Application information:
I (524) app_init: Project name:     wifi_prov_mgr
I (529) app_init: App version:      1
I (534) app_init: Compile time:     Sep 26 2024 13:38:07
I (540) app_init: ELF file SHA256:  bd58eaf41...
I (545) app_init: ESP-IDF:          v5.3.1
I (550) efuse_init: Min chip rev:     v0.0
I (554) efuse_init: Max chip rev:     v3.99
I (559) efuse_init: Chip rev:         v3.0
I (565) heap_init: Initializing. RAM available for dynamic allocation:
I (572) heap_init: At 3FFAFF10 len 000000F0 (0 KiB): DRAM
I (578) heap_init: At 3FFB6388 len 00001C78 (7 KiB): DRAM
I (584) heap_init: At 3FFB9A20 len 00004108 (16 KiB): DRAM
I (590) heap_init: At 3FFC9F38 len 000160C8 (88 KiB): DRAM
I (596) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (602) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (609) heap_init: At 4009BFC0 len 00004040 (16 KiB): IRAM
I (617) spi_flash: detected chip: generic
I (620) spi_flash: flash io: dio
W (623) spi_flash: Detected size(4096k) larger than the size in the binary image header(2048k). Using the size in the binary image header.
I (638) coexist: coex firmware version: 4482466
I (643) main_task: Started on CPU0
I (653) main_task: Calling app_main()
I (683) wifi:wifi driver task: 3ffcdd9c, prio:23, stack:6656, core=0
I (683) wifi:wifi firmware version: ccaebfa
I (683) wifi:wifi certification version: v7.0
I (683) wifi:config NVS flash: enabled
I (683) wifi:config nano formating: disabled
I (693) wifi:Init data frame dynamic rx buffer num: 32
I (693) wifi:Init static rx mgmt buffer num: 5
I (703) wifi:Init management short buffer num: 32
I (703) wifi:Init dynamic tx buffer num: 32
I (703) wifi:Init static rx buffer size: 1600
I (713) wifi:Init static rx buffer num: 10
I (713) wifi:Init dynamic rx buffer num: 32
I (723) wifi_init: rx ba win: 6
I (723) wifi_init: accept mbox: 6
I (723) wifi_init: tcpip mbox: 32
I (733) wifi_init: udp mbox: 6
I (733) wifi_init: tcp mbox: 6
I (733) wifi_init: tcp tx win: 5760
I (743) wifi_init: tcp rx win: 5760
I (743) wifi_init: tcp mss: 1440
I (753) wifi_init: WiFi IRAM OP enabled
I (753) wifi_init: WiFi RX IRAM OP enabled
I (763) wifi_prov_scheme_ble: BT memory released
I (763) app: Starting provisioning
I (773) app: Development mode: using hard coded salt
I (773) app: Development mode: using hard coded verifier
I (783) phy_init: phy_version 4830,54550f7,Jun 20 2024,14:22:08
I (863) wifi:mode : sta (94:b5:55:f2:65:8c)
I (863) wifi:enable tsf
I (863) BTDM_INIT: BT controller compile version [b022216]
I (873) BTDM_INIT: Bluetooth MAC: 94:b5:55:f2:65:8e
I (1103) protocomm_nimble: BLE Host Task Started
I (1113) wifi_prov_mgr: Provisioning started with service name : PROV_F2658C 
I (1113) app: Provisioning started
I (1123) app: Scan this QR code from the provisioning application for Provisioning.
I (1123) QRCODE: Encoding below text with ECC LVL 0 & QR Code Version 10
I (1133) QRCODE: {"ver":"v1","name":"PROV_F2658C","username":"wifiprov","pop":"abcd1234","transport":"ble"}
I (1153) NimBLE: GAP procedure initiated: advertise;
I (1153) NimBLE: disc_mode=2
I (1153) NimBLE:  adv_channel_map=0 own_addr_type=0 adv_filter_policy=0 adv_itvl_min=256 adv_itvl_max=256
I (1163) NimBLE:


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


I (1433) app: If QR code is not visible, copy paste the below URL in a browser.
https://espressif.github.io/esp-jumpstart/qrcode.html?data={"ver":"v1","name":"PROV_F2658C","username":"wifiprov","pop":"abcd1234","transport":"ble"}
I (8763) app: BLE transport: Connected!
I (8973) protocomm_nimble: mtu update event; conn_handle=0 cid=4 mtu=256
I (10653) security2: Using salt and verifier to generate public key...
I (11283) app: Secured session established!
W (116503) wifi:Password length matches WPA2 standards, authmode threshold changes from OPEN to WPA2
I (116533) app: Received Wi-Fi credentials
        SSID     : AIS 4G Hi-Speed Home WiFi_76947550769475
        Password : 50769475
I (122633) wifi:new:<11,0>, old:<1,0>, ap:<255,255>, sta:<11,0>, prof:1, snd_ch_cfg:0x0
I (122643) wifi:state: init -> auth (0xb0)
I (122643) wifi:state: auth -> assoc (0x0)
I (122663) wifi:state: assoc -> run (0x10)
I (122683) wifi:connected with AIS 4G Hi-Speed Home WiFi_769475, aid = 6, channel 11, BW20, bssid = 30:0a:c5:9e:94:9f
I (122683) wifi:security: WPA2-PSK, phy: bgn, rssi: -52
I (122703) wifi:pm start, type: 1

I (122703) wifi:dp: 1, bi: 102400, li: 3, scale listen interval from 307200 us to 307200 us
I (122763) wifi:AP's beacon interval = 102400 us, DTIM period = 1
I (128203) app: Connected with IP Address:192.168.1.155
I (128203) esp_netif_handlers: sta ip: 192.168.1.155, mask: 255.255.255.0, gw: 192.168.1.1
I (128203) wifi_prov_mgr: STA Got IP
I (128213) app: Provisioning successful
I (128213) app: Hello World!
I (129213) app: Hello World!
I (130213) app: Hello World!
I (131213) app: Hello World!
I (132213) app: Hello World!
I (133013) NimBLE: GAP procedure initiated: stop advertising.

I (133023) NimBLE: GAP procedure initiated: stop advertising.

I (133023) NimBLE: GAP procedure initiated: terminate connection; conn_handle=0 hci_reason=19

E (133093) protocomm_nimble: Error setting advertisement data; rc = 30
I (133103) wifi_prov_mgr: Provisioning stopped
I (133103) app: BLE transport: Disconnected!
I (133103) wifi_prov_scheme_ble: BTDM memory released
I (133213) app: Hello World!
I (134213) app: Hello World!
I (135213) app: Hello World!
I (136213) app: Hello World!
I (137213) app: Hello World!
I (138213) app: Hello World!
I (139213) app: Hello World!
I (140213) app: Hello World!
I (141213) app: Hello World!
I (142213) app: Hello World!
I (143213) app: Hello World!
I (144213) app: Hello World!
I (145213) app: Hello World!
I (146213) app: Hello World!
I (147213) app: Hello World!
I (148213) app: Hello World!
I (149213) app: Hello World!
I (150213) app: Hello World!
I (151213) app: Hello World!
I (152213) app: Hello World!
I (153213) app: Hello World!
I (154213) app: Hello World!
I (155213) app: Hello World!
I (156213) app: Hello World!
I (157213) app: Hello World!
I (158213) app: Hello World!
I (159213) app: Hello World!
I (159433) wifi:<ba-add>idx:0 (ifx:0, 30:0a:c5:9e:94:9f), tid:0, ssn:7, winSize:64
I (160213) app: Hello World!
I (161213) app: Hello World!
I (162213) app: Hello World!
I (163213) app: Hello World!
I (164213) app: Hello World!
I (165213) app: Hello World!
I (166213) app: Hello World!
I (167213) app: Hello World!
I (168213) app: Hello World!
I (169213) app: Hello World!
I (170213) app: Hello World!
I (171213) app: Hello World!
I (172213) app: Hello World!
I (173213) app: Hello World!
I (174213) app: Hello World!
I (175213) app: Hello World!
I (176213) app: Hello World!
I (177213) app: Hello World!
I (178213) app: Hello World!
I (179213) app: Hello World!
I (180213) app: Hello World!
I (181213) app: Hello World!
I (182213) app: Hello World!
I (183213) app: Hello World!
I (184213) app: Hello World!
I (185213) app: Hello World!
I (186213) app: Hello World!
I (187213) app: Hello World!
I (188213) app: Hello World!
I (189213) app: Hello World!
I (190213) app: Hello World!
I (191213) app: Hello World!
I (192213) app: Hello World!
I (193213) app: Hello World!
I (194213) app: Hello World!
I (195213) app: Hello World!
I (196213) app: Hello World!
I (197213) app: Hello World!
I (198213) app: Hello World!
I (199213) app: Hello World!
I (200213) app: Hello World!
I (201213) app: Hello World!
I (202213) app: Hello World!
I (203213) app: Hello World!
I (204213) app: Hello World!
I (205213) app: Hello World!
I (206213) app: Hello World!
I (207213) app: Hello World!
I (208213) app: Hello World!
I (209213) app: Hello World!
I (210213) app: Hello World!
I (211213) app: Hello World!
I (212213) app: Hello World!
I (213213) app: Hello World!
I (214213) app: Hello World!
I (215213) app: Hello World!
I (216213) app: Hello World!
I (217213) app: Hello World!
I (218213) app: Hello World!
I (219213) app: Hello World!
I (220213) app: Hello World!
I (221213) app: Hello World!
I (222213) app: Hello World!
I (223213) app: Hello World!
I (224213) app: Hello World!
I (225213) app: Hello World!
I (226213) app: Hello World!
I (227213) app: Hello World!
I (228043) wifi:<ba-add>idx:1 (ifx:0, 30:0a:c5:9e:94:9f), tid:6, ssn:0, winSize:64
I (228213) app: Hello World!
I (229213) app: Hello World!
I (230213) app: Hello World!
I (231213) app: Hello World!
I (232213) app: Hello World!
I (233213) app: Hello World!
I (234213) app: Hello World!
I (235213) app: Hello World!
I (236213) app: Hello World!
I (237213) app: Hello World!
I (238213) app: Hello World!
I (239213) app: Hello World!
I (240213) app: Hello World!
I (241213) app: Hello World!
I (242213) app: Hello World!
I (243213) app: Hello World!
I (244213) app: Hello World!
I (245213) app: Hello World!
I (246213) app: Hello World!
I (247213) app: Hello World!
I (248213) app: Hello World!
I (249213) app: Hello World!
I (250213) app: Hello World!
I (251213) app: Hello World!
I (252213) app: Hello World!
I (253213) app: Hello World!
I (254213) app: Hello World!
I (255213) app: Hello World!
I (256213) app: Hello World!
I (257213) app: Hello World!
I (258213) app: Hello World!
I (259213) app: Hello World!
I (260213) app: Hello World!
I (261213) app: Hello World!
I (262213) app: Hello World!
I (263213) app: Hello World!
I (264213) app: Hello World!
I (265213) app: Hello World!
I (266213) app: Hello World!
I (267213) app: Hello World!
I (268213) app: Hello World!
I (269213) app: Hello World!
I (270213) app: Hello World!
I (271213) app: Hello World!
I (272213) app: Hello World!
I (273213) app: Hello World!
I (274213) app: Hello World!
I (275213) app: Hello World!
I (276213) app: Hello World!
I (277213) app: Hello World!
I (278213) app: Hello World!
I (279213) app: Hello World!
I (280213) app: Hello World!
I (281213) app: Hello World!
I (282213) app: Hello World!
I (283213) app: Hello World!
I (284213) app: Hello World!
I (285213) app: Hello World!
I (286213) app: Hello World!