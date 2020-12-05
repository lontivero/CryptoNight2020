---
marp: true
title: WabiSabi
description: El desafío de la privacidad adopción y la escalabilidad
theme: uncover
_paginate: false
---

<!-- size: 19:6 -->


![bg 30% blur](./images/logo.png)

##### <!--fit--> Wasabi Wallet 


*El desafío de la privacidad: adopción y la escalabilidad*


<style scoped>a { color: #eee; }</style>

<!-- This is presenter note. You can write down notes through HTML comment. -->

---

![bg](#123)
![](#fff)

##### <!--fit--> 👉 Imagina un bitcoin a

##### <!--fit--> $100,000 :dollar: 

¿Cómo afectaría esto a las soluciones de privacidad?

---

# Soluciones actuales

* Coinjoin con uno mismo
* Coinjoin con quien recibe (payjoin)
* Fake conjoins
* Coin swaps

<br>

Requieren de múltiples transacciones on-chain: Costosas

---

# ¿Qué es una tx coinjoin?

![width:800px](./images/transactions.png)

![width:400px](./images/coinjoin.png)

---
# Mejora la privacidad

![width:800px](./images/sub_transactions.png)

---

## Knapsack (1)

![bg right width:400px](./images/knapsack_transaction.png)

* Siete participantes máximo
* Coinjoin o lote de transacciones
* Posibles subtransacciones posibles: 32.004 


----------

# Knapsack

* Transacciones válidas: 45
* Suficiente ambiguedad

![width:600px](./images/knapsack_analysis.png)

<style scoped>
h3 { font-size: 24px; }
p {
  font-size: 24px;
}
</style>

**Ejemplo:** Wasabi CJ 58 inputs - 112 outputs (2) **~374144419156711147060143317175368453031918731001856** subtransacciones 

---

# Desafíos 

* Eficiancia de espacio

   * Menos transacciones
   * Mayor grado de anonimato por unidad de espacio
   * Menos outputs (outputs pequeños)

---

# Desafíos 

* Eficiancia de tiempo

   * Mayor liquidez (eliminar restricciones de montos)
   * Mayor grado de ambiguedad
   * Menos outputs (menos outputs pequeños)

---


## WabiSabi

Una generalización del protocolo Chaumian CoinJoin basado en un esquema keyed-verification anonymous credentials (KVAC).

---

## WabiSabi


* Pagos a través de conjoins
* Pagos anónimos
* Payjoins en coinjoins

---

## WabiSabi lotes

![batching](./images/batching.png)

---

## WabiSabi sin cambio

![batching](./images/amount_fee.png)

---

### <!--fit--> :pray:

---

### <!--fit--> :question:

---


## **[WabiSabi Research Club Review](https://github.com/zkznacks/WabiSabi)**

1. [Anonymous CoinJoin Transactions with Arbitrary Values](https://www.comsys.rwth-aachen.de/fileadmin/papers/2017/2017-maurer-trustcom-coinjoin.pdf)

2. [WabiSabi - A generalization of Chaumian CoinJoin based on a KVAC scheme](https://github.com/zkSNACKs/WabiSabi/releases/latest/download/WabiSabi.pdf)
---

![bg 30% opacity blur](./images/lontivero.png)

### Lucas Ontivero ([@lontivero](https://github.com/lontivero))

https://github.com/zksnacks/walletwasabi

