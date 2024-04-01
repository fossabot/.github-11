# openEBS
[![OpenEBS Social Banner](https://github.com/openebs/website/blob/main/website/public/images/png/openebs_github_main_banner_HERO_1.png)](https://www.openebs.io/)

# [openebs.io](https://www.openebs.io/)
OpenEBS is a free openesource Stateful Persistent Data Storage platform for Kubernetes. We are CNCF member project. We are a large global community of K8s Datastorage users.<BR>
<BR>
Our project team was an early pioneering inventor of K8s **Container Native Storage** services. We concieved the vision of a K8s Stateful Persistent data platform that is tightly integrated and embeded natively into the core of K8s.<BR>
<BR>
We have designd and built an innovative ultra High-performance Enterprise grade Block-mode storage Hyper-converged Data Fabric that augments the core storage services of K8s with Stateful Persistence, Enterprise Data mgmt, SSD/NVMe optimized I/O services,
Replicated Data volumes, Thin Provisioning, Snapshot and Clones; and many other critical data storage services that don't come in K8s out-of-the-box.<BR>
<BR>
Building an Enterprise Data Storage platform is complex, and areas of the Data & I/O stack could be considerd 'Rocket science'. Our global team comes from many areas of the data storage industry and our project is sponsored by many innovative data storage companies within the industry, as well as many amazing individuals. Coding, contribuing, brainstorming ideas to the project are all welcome.<BR>
<BR>
<BR>
## Project structure
As a project, OpenEBS hasmaintained a steady pace of evolution in order to keep in alignment with K8s advancment overall and with the rapid changing pace of technologies, hardware and software innovations in the data stroage industry. The proejct is divided into 2 main deployable Editions :<BR>
| ID  | Edition name  |
|-----|---------------|
|  1  |  Legacy       |
|  2  |  Standard     |
<BR>

## LEGACY
LEGACY consists of Data-Engines that we experimented with early on. These Data-Engines have a number of opensoruce techologies embeded inside them, and are a great intro into the world of simple K8s storage services. LEGACY helped us learn, iterate and develop our core storage K8s strategy, as well as decern how users want & need to interact with K8s storage services. LEGACY also helped to reveal key areas within K8s that are lacking in storage/datastore services,  what areas of K8s we could optimize; and how we can provide the best value into the various K8s storage layers.<BR>
<BR>
There are multiple Data-Engines within LEGACY:<BR>
| ID  | Data-Eegines      | Embeded tech stack   | Status                           |
|-----|-------------------|----------------------|----------------------------------|
|  1  |  Jiva             | iSCSI                | We plan to sunset LEGACY in 2024 |
|  2  |  cStor            | Open ZFS             | We plan to sunset LEGACY in 2024 |
|  3  |  NFS Provisioner  | NFS userspace server | We plan to sunset LEGACY in 2024 |
|  4  |  Device LocalPV     | Node Local storage   | We plan to sunset LEGACY in 2024 |
|  5  |  LocalPV Device     | Node Local storage   | We plan to sunset LEGACY in 2024 |
|  6  |  NDM              | Node Local storage   | We plan to sunset LEGACY in 2024 |
|  7  |  Many other tools   | Node Local storage   | We plan to sunset LEGACY in 2024 |

<BR>

## STANDARD
**STANDARD** is our Ultra modern Datastore stack that is strongly aligned with the cutting edge direction of storage use-cases in the K8s industry. It is designed to faciliate modern K8s datastore archiectures, key K8s I/O patterns, K8s data access methods, K8s data use-cases and where K8s Datastore applications are heading.
* STANDARD is optimized for NVMe and SSD Flash and integrates ultra modern extremme high performance storage technologies at its core...
    * It uses the High performance [SPDK](https://spdk.io) storage stack - (SPDK is an opensource NVMe project initiated by INTEL)
    * The hyper modern [IO_Uring](https://github.com/axboe/liburing) Linux Kernel Async polling-mode I/O Interface - (fastest kernel I/O mode possible)
    * Native abilties for RDMA and Zero-Copy I/O
    * NVMe-oF TCP Block storage Hyper-converged data fabric
    * Block layer volume replication
    * Logical volumes and Diskpool based data managment
    * a Native high peformance Blobstore
    * Native Block layer Thin provisoning
    * Native Block layer Snapshtos and Clones
 <BR>	

**STANDARD** Edition groups its Data-Engines into 2 main core types of storage services:
- Replicated
- Local (Non-replicated(

| ID  | Data-Eegines       | Type of data services                                  | Status                                                     |
|-----|--------------------|--------------------------------------------------------|------------------------------------------------------------|
|  1  |  ```Replciated``` <BR>**Mayastor**      | Replicated data volumes (a Cluster wide Data fabric)   | Stable, deployable in PROD. Very active development        |
|     | &nbsp;             |                                                        |                                                            |
|    | ```Local``` <BR>**LocalPV-xxx**      | Non-replicated node local data volumes                 | (see multiple variants below...)                         |
|  2   |  LocalPV-LVM      | for integration with LVM datastor deployments          | Stable, deployable in PROD, undergoing integration         |
|  3   |  LocalPV-ZFS      | for integration with ZFS datastor deployments          | Stable, deployable in PROD, undergoing integration         |
|  4   |  LocalPV-HostPath | for integration with local node hostpath (/mnt/fs1)    | Stable, deployable in PROD, undergoing integration         |
|  5   |  LocalPV-RawFile    | for integration with Soft-Lun Block Device files that reside on a node local filesystem ( Loop Device mounted) | Stable, deployable in PROD, undergoing integration         |
<BR>


## ROADMAP
Our [2024 Roadmap is here](https://github.com/openebs/openebs/blob/main/ROADMAP.md) It defines a rich set of new featrues that are planned for 2024.<br>
Please review this roadmp and feel free to pass back any feedback on it, as well as recommend and suggest new ideas. We welcome all your feedback.
<br>
<br>

## GitHub Star Chart
OpenEBS is the most successful Stateful Persistent Contianer Native Storage platform in the CNCF landscape. It has allways held the #1 position and continues to as of today.
[![XXXXXXXX](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png)](https://www.openebs.io/)
