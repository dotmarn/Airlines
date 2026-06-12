# Airlines 🔀

This repository is a fork of https://github.com/dotmarn/Airlines.

## Passenger.json

In this version you will find the ```passenger.json``` file which includes only the main **active passenger** airlines.

Many airlines in the original list have ceased their operations, or they are not airlines but bus or rail companies
instead. Also, a lot of them are minor regional airlines or ghost airlines.
**All these airlines/companies are not included in ```passenger.json```**.

**Note on exclusively or mainly charter airlines:**
since it's not easy to determine which is the perimeter of operation of these airlines, they were also omitted in
```passenger.json```.

**Note on leasing airlines:**
leasing airlines uses an IATA code that rarely appears on the final passenger's ticket so there is no need to keep them
in the list.

Some airlines names or codes from ```passenger.json``` may differ from the ones in ```airlines.json``` because they have
been updated based on the latest market operations (renaming, merges, rebranding, etc.).

You can also use ```passenger.min.json``` that is ~14KB less.

_If you need cargo, charter, leasing or defunct airlines, please refer to airlines.json._

# Contributing

This repo is open to anyone who wants to contribute.
You can update or remove existing airlines, add new ones and create new jsons for better grouping.

### Contribution requirements:

If you're editing existing files please keep always the same format:

```
{
    "iata": string //IATA code (see * below)
    "lcc": string //Low Cost Carrier; must be 0/1/None
    "name": string //Airline brand name; not the company name (see ** below)
    "logo": string //Airline logo; must square sized, at least 64x64 px.
}
```

\* IATA code must be previously checked on https://www.iata.org/en/publications/directories/code-search/ <br>
\** Official company's name, sometimes is different from the name with which the airline is recognised so the brand name
must be used.

If you want to add a new field to the airlines, make sure to add it for all the airlines.

When you're creating a new file feel free to decide the data format but keep it consistent throughout all the list
items.

___

## Roadmap

- [ ] periodically (every 6 months) update with the new passenger airlines
- [ ] add cargo.json
- [ ] add icao codes in passenger.json
- [ ] add missing Asian airlines
- [ ] add missing Southern American airlines
- [ ] add missing Russian airlines
- [ ] add missing African airlines

___

#### Original README.md below ⤵️

This repository offers the resources to all airlines (over 500) including their flags/logo in a JSON file.

### Some of the available airlines

![Arik](https://images.kiwi.com/airlines/64/W3.png)
![Saudi](https://images.kiwi.com/airlines/64/SV.png)
![Atlantic](https://images.kiwi.com/airlines/64/RC.png)
![Virgin Atlantic](https://images.kiwi.com/airlines/64/VS.png)
![British Airways](https://images.kiwi.com/airlines/64/BA.png)

___ 

# Airlines Changelog

- ### 2025.09.12:
  initial commit; removed old, cargo, charter, leasing, ghost airlines; added XZ, SV, XN.
- ### 2025.09.13:
  changed non-IATA SZS to SZ; removed DI, 8Z, K2; added W4, FV, D8, N0 
