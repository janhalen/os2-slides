flowchart LR
 subgraph s1["Repositorier"]
        source1["Kildekode"]
        source2["Kildekode"]
        source3["Kildekode"]
  end
 subgraph s3["Eksterne afhængigheder"]
        source4["Afhængighed"]
  end
 subgraph s2["Repositorier"]
        U["Udrulning"]
  end
 subgraph i1["Instans1"]
        infra1["Infrastruktur"]
        app1["Applikation"]
  end
 subgraph i2["Instans2"]
        infra2["Infrastruktur"]
        app2["Applikation"]
  end
 subgraph i3["Instans3"]
        infra3["Infrastruktur"]
        app3["Applikation"]
  end
    app1 -.- infra1
    app2 -.- infra2
    app3 -.- infra3
    source1 --> B["Byg + Pak + Test"]
    source2 --> B
    source3 --> B
    B --> I(("Udgivelse"))
    I -....- U
    U --> i1 & i2 & i3
    source4 -.- n1["Small Circle"]
    n1 --> B
    n1 -.- source3

    source1@{ shape: card}
    source2@{ shape: card}
    source3@{ shape: card}
    U@{ shape: card}
    infra1@{ shape: loop-limit}
    app1@{ shape: display}
    infra2@{ shape: manual-input}
    app2@{ shape: display}
    infra3@{ shape: trap-b}
    app3@{ shape: display}
    B@{ shape: h-cyl}
    n1@{ shape: sm-circ}
     infra1:::Class_01
     app1:::Aqua
     infra2:::Class_02
     app2:::Aqua
     infra3:::Class_03
     app3:::Aqua
    classDef Aqua stroke-width:1px, stroke-dasharray:none, stroke:#46EDC8, fill:#DEFFF8, color:#378E7A
    classDef Class_02 fill:#09ffc1, stroke:#BBDEFB
    classDef Class_01 fill:#5cc9ff, stroke:#BBDEFB
    classDef Class_03 fill:#ba8bf496, stroke:#BBDEFB
    style source1 stroke:#C8E6C9
    style source2 stroke:#FFE0B2
    style source3 stroke:#E1BEE7
    style source4 stroke:#757575
    style U stroke:#757575
    style infra2 stroke:#C8E6C9
    style infra3 stroke:#E1BEE7
    style B stroke:#757575
    style I stroke:#BBDEFB
    style i1 stroke:#BBDEFB
    style i2 stroke:#C8E6C9
    style i3 stroke:#E1BEE7
    style s1 stroke:none
    style s3 stroke:none
    style s2 stroke:none
    linkStyle 3 stroke:#757575,fill:none
    linkStyle 4 stroke:#757575,fill:none
    linkStyle 5 stroke:#757575,fill:none
    linkStyle 6 stroke:#757575,fill:none
    linkStyle 8 stroke:#757575,fill:none
    linkStyle 9 stroke:#757575,fill:none
    linkStyle 10 stroke:#757575,fill:none
    linkStyle 12 stroke:#757575,fill:none


