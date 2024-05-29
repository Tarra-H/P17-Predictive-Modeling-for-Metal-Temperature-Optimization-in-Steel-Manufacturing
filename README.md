# Predictive-Modeling-for-Metal-Temperature-Optimization-in-Steel-Manufacturing

**Project Description**

- In an effort to optimize production costs, the Steelproof steel plant has ultimately decided to reduce energy consumption during the steel processing stage. Thus, to assist in this decision, the company has commissioned us to create and develop a machine learning model that can predict metal temperature.
- To create a good model, we must also understand the steps of steel processing. Here is an overview:
  1. Steel is processed in a metal ladle with a capacity of about 100 tons. To withstand very high temperatures, the ladle is lined with refractory bricks on its inner surface. Then, molten steel is poured into the ladle and heated to the desired temperature using graphite electrodes located in its lid. Graphite electrodes are used to heat the metal in the ladle by passing an electric current through them.
  2. Sulfur is removed from the metal through the desulfurization process. The chemical composition of the steel is corrected (by adding alloy in the form of bullion from bulk material bunkers or with the help of wire feeders), and then the required samples are taken.
  3. Before alloying elements are added, the temperature of the steel is measured, and its chemical composition is analyzed. The temperature is then raised for a few minutes, alloying elements are added, and the alloy is cleaned with inert gas. After that, the alloy is stirred and its temperature is measured again. This cycle is repeated until the optimal chemical composition and melting temperature are achieved.
  4. The molten steel is then refined or transferred to a continuous casting machine where it solidifies into steel slabs.

**Objective:**

The goal of this work is to create and develop a machine learning model that can predict metal temperature.

**Data:**

The dataset is located in the final_steel_en.zip folder with the path /datasets/final_steel_en/.

**Data Description:**

The data consists of files obtained from various sources:

- 'data_arc.csv' — electrode data
- 'data_bulk.csv'  — bulk material supply data (volume)
- 'data_bulk_time.csv' — bulk material delivery data (time)
- 'data_gas.csv' — gas flushing data
- 'data_temp.csv' — temperature measurement results
- 'data_wire.csv' — wire material data (volume)
- 'data_wire_time.csv' — wire material data (time)

In each file, the key column contains the batch number.

There may be several rows with the same 'key' value in these files.

These values correspond to different processing iterations.

**With Requirements:**
- Target Feature: last measured temperature
- Metric: MAE
- Evaluation Criteria:
    - MAE > 8.7 — 0 SP
    - 7.6 < MAE ≤ 8.7 — 4 SP
    - 6.8 < MAE ≤ 7.6 — 4.5 SP
    - 6.3 < MAE ≤ 6.8 — 5 SP
    - 6.0 < MAE ≤ 6.3 — 5.5 SP
    - MAE ≤ 6.0 —  6 SP
