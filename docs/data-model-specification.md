# Data-model

Data schema by example.

## Verionn 1

```
[

    {
        name: "Test-Route-1",
        from: "Berlin",
        to: "Munich",
        vehicle_type: "BMW i3"
        consumption_percentage: 45,
        waypoints: [
            {
                lon:14.4,
                lat:16.3,
                speed: 83,
                ...
            }
        ]

    },

    {
        name: "Test-Route-2",
        from: "Berlin",
        to: "Munich",
        vehicle_type: "BMW i3"
        consumption_percentage: 45,
        waypoints: [
            {
                lon:14.4,
                lat:16.3,
                speed: 83,
                ...
            }
        ]

    },

]
```

## Version 2

```
[

    {
        name: "Test-Route-1",
        from: "Berlin",
        to: "Munich",
        vehicle_type: "BMW i3,

        sections: [
            {
                name: "Test-Route-1",
                consumption_percentage: 10,
                waypoints: [
                    {
                        lon:14.4,
                        lat:16.3,
                        speed: 83,
                        ...
                    }
                ]
            },
            ...
        ]

    },

    {
        name: "Test-Route-2",
        from: "Berlin",
        to: "Munich",
        vehicle_type: "BMW i3"

        sections: [
            {
                name: "Test-Route-2-s1",
                consumption_percentage: 10,
                waypoints: [
                    {
                        lon:14.4,
                        lat:16.3,
                        speed: 83,
                        ...
                    }
                ]
            },
            ...
        ]

    },

    ...

]

```