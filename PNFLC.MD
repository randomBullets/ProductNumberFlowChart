graph TD
    A[Start] --> B{Select Model}
    B -->|E120| C1[E120]
    B -->|EN120| C2[EN120]
    B -->|E90| C3[E90]
    B -->|EN90| C4[EN90]
    B -->|E60| C5[E60]
    B -->|EN60| C6[EN60]

    C1 & C2 & C3 & C4 & C5 & C6 --> D{Select Voltage}
    D -->|Option 1| E1[Voltage 1]
    D -->|Option 2| E2[Voltage 2]
    D -->|Option 3| E3[Voltage 3]

    E1 & E2 & E3 --> F{Select Number of Internal Mini Units}
    F -->|E120/EN120| G1{3-8 units}
    F -->|E90/EN90| G2{3-6 units}
    F -->|E60/EN60| G3{3-4 units}

    G1 --> H1[3 units]
    G1 --> H2[4 units]
    G1 --> H3[5 units]
    G1 --> H4[6 units]
    G1 --> H5[7 units]
    G1 --> H6[8 units]

    G2 --> I1[3 units]
    G2 --> I2[4 units]
    G2 --> I3[5 units]
    G2 --> I4[6 units]

    G3 --> J1[3 units]
    G3 --> J2[4 units]

    H1 & H2 & H3 & H4 & H5 & H6 & I1 & I2 & I3 & I4 & J1 & J2 --> K[Generate Part Number]
    K --> L[End]
