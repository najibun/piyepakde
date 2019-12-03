# REPO TUGAS KELOMPOK TCC
Anggota :   
Muhammad Najib  
Rizky Harya R  
Andri Siswanto  
Lukman Surya Laksana  
Dzikry Kusuma  

## Konsep
![alt text](IMG11/1.jpg)

Gambar diatas adalah salah satu layanan IAAS. Disitu terlihat bahwa layanan cloud IaaS akan menyediakan satu unit berupa (lihat nomor diatas);

1. Sistem operasi – sistem operasi yang dipilih seperti Debian, Centos, Ubuntu dan semua OS Linux. 
2. Nama – disini adalah nama server virtual
3. IP Address – pihak penyedia memberikan IP Address
4. Status Active – ini adalah menu untuk mengaktifkan atau menonaktifkan server
5. Memory, ini adalah layanan RAM yang berbeda-beda sesuai dengan spesifikasi yang dipilih, bisa 512MB, 1GB, 2GB dan seterusnya
6. Disk – dalam hal ini adalah tempat penyimpanan data, sama dengan 
7. RAM, disesuaikan dengan spesifikasi yang dipilih
Region – ini adalah zona dimana kita memilih tempat. Ini digunakan sebagai alamat DNS. Terkadang sangat penting untuk bisnis online dengan target negara tertentu.

Dengan spesifikasi tersebut Anda bisa menginstal dengan banyak pilihan sistem operasi, setelah anda instal kemudian pihak vendor juga menyediakan hal-hal yang mendukung satu unit yang Anda “sewa” baik perjam atau perbulan itu agar terkoneksi dengan internet secara realtime. Sehingga kapan saja, Anda butuh data pada satu unit yang Anda pesan, Anda bisa mendownload kapan saja.

Sifat elastis dari produk cloud computing memungkinkan para wirausahawan teknologi untuk menggunakan anggaran sesuai kebutuhan, agar stabilitas operasional bisnis tetap terjaga dan berimbang.

## Berbagai sofware IaaS
1. Amazon, Inc – Amazon EC2

   ![alt text](img/amazon.png)

   Amazon EC2 dalah platform komputasi berupa virtual computer yang dapat di kustomisasi maupun di kembangkan dengan menggunakan prinsip cluster dan load balance. Untuk deployment nya sendiri sangat mudah sekali karena hanya perlu memilih image yang disebut AMI (Amazon Machine Instances) dan setup hanya perlu 5-10 menit.


2. Telkom – TelkomCloud

   ![alt text](img/telkom_cloud.jpg)

   TelkomCloud adalah layanan yang menyediakan IT Resources Service (Computing, Storage & Network) dan Application Services dengan menggunakan teknologi virtualisasi berbasis cloud computing (on-demand, rapid elasticity, & fast deployment) yang akan meningkatkan akselerasi bisnis pelanggan.


3. NaviSite, Inc.

   ![alt text](img/navisite.png)

   Merupakan Time Warner Cable Company, adalah penyedia internasional terkemuka dari pelayanan dan pengaturan aplikasi-aplikasi kelas enterprise dan hosting cloud. NaviSite menyediakan rangkaian lengkap dari layanan yang dikelola serta dapat diandalkan dan terukur, termasuk pelayanan aplikasi, Hosting perusahaan yang terdepan dalam industri, dan pelayanan pengaturan Cloud untuk organisasi ingin melakukan outsourcing infrastruktur TI dan membantu menurunkan modal serta biaya operasional. Konsumen perusahaan bergantung pada NaviSite untuk solusi khusus, yang disampaikan melalui pusat data kelas internasional yang canggih.

## Getting started PROXMOX  
Proxmox VE merupakan kependekan dari Proxmox Virtual Environment ada juga yang mengingkat menjadi PVE. Pengertian dari Proxmox VE adalah suatu platform virtualisasi yang stabil, lengkap, memiliki team support yang baik dan masuk di kelas virtualisasi enterprise. Proxmox ini merupakan proyek open source, dibangun dari Linux Debian. Proxmox VE akan melakukan manajeme container, virtual machine, storage, jaringan virtual, high availability cluster melalui antar muka web dan dapat juga menggunakan command line.  

PVE ini juga dikenal sebagai type hypervisor. Hypervisor ini merupakan aplikasi yang dapat melakukan manajemen virtual machine. Hypervisor dapat membuat virtual machine ,  melakukan konfigurasi virtual machine, menjalankan virtual machine dan juga mengendalikan virtual machine ini.  

Proxmox VE ini merupakan type 2 hypervisor. Type 2 hypervisor adalah hypervisor yang berjalan di atas operating system. Sedangkan type 1 hypervisor adalah hypervisor yang langsung menangani perangkat keras tanpa melalui operating system.  

Proxmox VE menggunakan Linux Debian karena Linux Debian mempertimbangkan release pada saat versi tersebut mencapai stability, security dan usability yang baik. Dengan demikan maka Proxmox VE mengandalkan Linux Debian dalam komitmentnya dalam stability, security, dan usability.  

Proxmox VE menyediakan teknologi virtualisasi yaitu  

1. KVM  
KVM merupakan kependekan dari Kernel Virtual Machine. KVM merupakan bagian integral dari Linux sejak tahun 2007.
Informasi lebih lanjut mengenai KVM silahkan mengunjungi http://www.linux-kvm.org/.  
2. QEMU  
QEMU menyediakan emulasi dan virtualisasi interface.
Informasi lebih lanjut mengenai QEMU dapat dibaca di http://www.qemu.org .  
3. LXC  
LXC atau Linux Container ini merupakan virtualisasi OS atau virtualisasi operating system. Di sini containernya diisolasi tetapi masih melakukan share pada operating system dan juga library/binnya.
Informasi lebih lanjut mengenai LXC silahkan mengunjungi https://linuxcontainers.org/ .

## Arsitektur dan konsep deplyment
![arsitektur1](./img/DIET_Proxmox_Archi.png)  
![arsitektur2](./img/DIET_Proxmox_Archi.png)
komponen arsitektur tersebut 
Cluster PVE : Several clustered servers PVE.
PVE : Hypervisor Proxmox.
API : Proxmox VE uses a REST like API. This API use JSON as data format. The whole API is formally defined using JSON Schema.  