# Draft Power Budget for VK2RRT

by James Cameron VK2LQZ<br>
14th March 2018


## Equipment Measurements

Received by e-mail and telephone conversation with Peter VK2BXQ.

* VHF receiver, 125 mA idle, 250 mA receive,
* VHF transmitter, 120 mA idle,
* repeater controller, 25 mA,
* UHF receiver and transmitter, 400 mA; note link with VK2RCD is blocked by terrain so this equipment will be off,
* solar regulator, 60 mA,
* two 90 W solar panels, total 180 W,
* wired in series at the moment.

## Generation Estimates

* assume nominal five hours insolation,
* total 900 WH per day, (180 &times; 5),

## Consumption Estimates

* idle current 0.33 A, 4.75 W, 114 WH per day,
* transmit current unknown, license limit 120 W, assume one hour per day, 120 WH per day,
* total 230 WH per day,

## Worst Case - No Sun

* check that there is capacity to cover multiple days overcast,
* typically 33% insolation; generation of 300 WH, consumption of 230 WH, plus losses,
* generation during overcast is sufficient to meet consumption assuming at least 230 WH of battery storage,
* generation on sunny days is more than three times consumption.

## Purchases recommended by Peter VK2BXQ and Brett VK2WWV

* [Giant 12V 130AH AGM Deep Cycle Battery](https://www.aussiebatteries.com.au/batteries/deep-cycle-agm/130ah-12v-agm-deep-cycle-battery) (aussiebatteries.com.au)
    * $270 each, quantity 3, quoted total $810,
    * Maximum temperature 40&deg;C,
    * Weight 31 kg each,

  calculations and review by James VK2LQZ,

    * Wire size 16mm&sup2;, 6AWG, for 40A maximum charge current, per [User Manual](http://www.epsolarpv.com/en/uploads/news/201710/1508813495487522.pdf),
    * Fuses &gt; 40A, e.g. 50A 5AG, quantity 2, between batteries,
        * protect a battery from another battery on cell fault,
    * Usable capacity at 10% DoD; 39 AH, 539 WH per day, 5 years, (not specified by retailer),
    * Battery life will be reduced by up to 50% due to temperature,
    * Emergency capacity 390 AH, 5382 WH, or 21 days with solar array down,
    * Battery life will be reduced by up to 90% if emergency capacity is ever used, or charge controller can disconnect loads before damage is done,
    * Meets requirements, but will have a short life due to temperature.

* [EPSOLAR Tracer4215BN MPPT charge controller](http://www.epsolarpv.com/en/index.php/Product/pro_content/id/573/am_id/136) (epsolarpv.com)

    * Already purchased as a donation by Peter,
    * Enclosure IP30,
    * Maximum temperature 55&deg;C,
    * Maximum input power 520 W (for a 12V nominal battery voltage),
    * Maximum charge current 40 A,
    * Low voltage cutoff 11.1 V,
    * Low voltage reconnect 12.6 V,
    * No maximum load current specification,
    * Assumes 25&deg;C for voltage temperature compensation when sensor not used,
    * [Datasheet](http://www.epsolarpv.com/en/uploads/news/201512/1449124059577504.pdf)
    * [User Manual](http://www.epsolarpv.com/en/uploads/news/201710/1508813495487522.pdf)

  calculations and review by James VK2LQZ,

    * Wire size 16mm&sup2;, 6AWG, for 40A maximum charge current, per [User Manual](http://www.epsolarpv.com/en/uploads/news/201710/1508813495487522.pdf),
    * Fuses &gt; 40A, e.g. 50A 5AG, quantity 1,
        * protect cable during charging,
        * protect cable on charger fault,
    * Charge current at 520 W input with battery at 11.1 V; 40 A,
    * Battery life can be increased by temperature sensor option RTS300R47K3.81A,
    * Battery life can be increased by low voltage cutoff and reconnect; so that if solar panels are covered, the system shuts down before the batteries are destroyed; requires configuring charger for manual load control, wiring repeater to load output, or for best transmit voltage wire a relay from the load output to the repeater controller,
    * Meets requirements,

* [Solar panels](http://www.lowenergydevelopments.com.au/solarpanels-poly-mono/solar-panels-upto-200w-morethan-100w/200-Watt-12v-Solar-Panel-Monocrystalline)

    * $147.50 each, quantity 3, total $442.50,
    * Maximum power 200W per panel, total of 600W,
    * Maximum open circuit voltage 22.0V, in series 66.0V,
    * Maximum short circuit current 12.12A, in series 12.12A,
    * Adapt frame for different panels, completed,
    * Fix frame to ground,
    * Retire existing panels,

  calculations and review by James VK2LQZ,

    * Wire size 6mm&sup2;, 10AWG, for 12.12A maximum short circuit current, or increase wire size for distance,
    * Panel total power exceeds maximum input power of charge controller, 600W vs 520W, but page 9 of charger manual says it will safely limit to the rated power,
    * System will complete charging within about 23 minutes of full sun,
    * Panels will be idle most of the day,
    * Exceeds requirements,

## Purchases recommended by James VK2LQZ

* [Sentry 40AH 12V](https://www.rpc.com.au/catalog/sentry-lithium-battery-40ah-12v-p-4588.html) (rpc.com.au)

    * $645,
    * Maximum temperature 50&deg;C,
    * Minimum temperature -20&deg;C,
    * Weight 5.5kg,
    * Maximum charge current 40A,
    * Contains a charge balancing battery management system,
    * [Datasheet](https://www.rpc.com.au/pdf/sentry_12V40S_datasheet.pdf),

  calculations,

    * Usable capacity at 100% DoD; 40AH, 552 WH per day, 5.5 years,
    * Emergency capacity same, or two days,
    * Meets requirements.

* [Victron SmartSolar MPPT Regulator 75/15](https://www.rpc.com.au/catalog/victron-smartsolar-mppt-regulator-75v-15a-p-4624.html) (rpc.com.au)

    * $186,
    * Enclosure IP43,
    * Maximum temperature 60&deg;C,
    * Maximum input power 440 W,
    * Maximum charge current 15 A,
    * Low voltage cutoff 11.1 V,
    * Low voltage reconnect 13.1 V,
    * [Datasheet](https://www.rpc.com.au/pdf/victron_SmartSolar_MPPT_75-100_10-20_datasheet.pdf).

  calculations,

    * Charge current at 180 W input with battery at 11.1 V; 15 A;

## Risks

* cable length of 35m does not seem right, trench was much shorter, suggested by Petria VK2FERE, see photograph,
* temperature can exceed 40&deg;C in shed; previous battery had enough thermal mass to avoid damage, but a small-celled AGM battery may not escape this.

----
