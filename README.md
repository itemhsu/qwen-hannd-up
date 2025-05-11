# qwen-hannd-up
A hands up guide with qwen local 
## Requirement
| 項目          | 指令             | 結果 |
|---------------|------------------|------------------|
| ubuntu 22.04 |  lsb_release -a | No LSB modules are available. <br>Distributor ID:	Ubuntu <br>Description: <br>Ubuntu 22.04.5 LTS <br>Release:	22.04 <br>Codename:	jammy|
|GPU RTX 3060 12G | sudo lshw -C display |<pre>   *-display                 <br>       description: VGA compatible controller<br>       product: GA106 [GeForce RTX 3060]<br>       vendor: NVIDIA Corporation<br>       physical id: 0<br>       bus info: pci@0000:01:00.0<br>       version: a1<br>       width: 64 bits<br>       clock: 33MHz<br>       capabilities: pm msi pciexpress vga_controller bus_master cap_list rom<br>       configuration: driver=nvidia latency=0<br>       resources: irq:136 memory:de000000-deffffff memory:c0000000-cfffffff memory:d0000000-d1ffffff ioport:e000(size=128) memory:c0000-dffff<br>  *-graphics<br>       product: EFI VGA<br>       physical id: 2<br>       logical name: /dev/fb0<br>       capabilities: fb<br>       configuration: depth=32 resolution=1024,768 </pre>|
| install ollama | curl -fsSL https://ollama.com/install.sh | run the sownload script |

## Run
ollama run qwen3:8b
| 功能          | 指令             | 
|---------------|------------------|
| 千問3基礎（無圖形）         | ollama run qwen3:8b        | 
| 千問3進階 （無圖形）          |ollama run qwen3:14b | 
| 千問2.5基礎 （圖形）          | ollama run ZimaBlueAI/Qwen2.5-VL-7B-Instruct |

Model pool : https://ollama.com/search?q=Qwen+VL

## List
```
itemhsu@i7:~/amtk$ ollama list
NAME                                        ID              SIZE      MODIFIED   
ZimaBlueAI/Qwen2.5-VL-7B-Instruct:latest    dccd480cacac    4.7 GB    6 days ago    
qwen3:14b
```
