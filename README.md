# GCP VM 管理器

本程式提供 GCP VM 的管理功能，包括啟動和停止虛擬機。

## 如何使用

使用前需先安裝 `gcloud` 工具，並且設定好相關的 GCP 帳戶和權限。

### 啟動 GCP VM

要啟動 GCP VM，執行以下命令：

```
python vm_manager.py --action start --num_vms <num_vms>
```

其中 `<num_vms>` 為要啟動的虛擬機數量。

### 停止 GCP VM

要停止 GCP VM，執行以下命令：

```
python vm_manager.py --action stop --vm_ids <vm_id_1> <vm_id_2> ... <vm_id_n>
```

其中 `<vm_id_1> <vm_id_2> ... <vm_id_n>` 為要停止的虛擬機 ID。可以指定多個虛擬機 ID，以空格分隔。

## 參數說明

### `--action`

要執行的操作，有兩個選項：`start` 和 `stop`。

### `--num_vms`

要啟動的 GCP VM 數量，只能在啟動 GCP VM 時使用。

### `--vm_ids`

要停止的 GCP VM ID，只能在停止 GCP VM 時使用。可以指定多個虛擬機 ID，以空格分隔。