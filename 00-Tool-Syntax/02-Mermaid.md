# Mermaid

## Orientation

`TD`
```mermaid
flowchart TD
  nodeId1 --> nodeId2
  nodeId3 --> nodeId4
```

---
`LR`
```mermaid
flowchart LR
  nodeId1 --> nodeId2
  nodeId3 --> nodeId4
```

---

`RL`
```mermaid
flowchart RL
  nodeId1 --> nodeId2
  nodeId3 --> nodeId4
```

## Node Text

```mermaid
flowchart LR
  id["text wrapped in double quotes displays content correctly more often"]
```

## Comments

```mermaid
flowchart LR
  %% this is a comment
  a["comments are lines starting with '%%'"]
```

## Node Shape

```mermaid
flowchart LR
  a[normal]
  b(round)
  c([stadium])
  f((circle))
  g{diamond}
```

## Edge Arrows

### Arrow Types

```mermaid
flowchart LR
  a  ---  b
  c  ===  d
  e   --> f
  g  <--> h
  i   ==> j
  k  <==> l
  m  -.-  n
  o  -.-> p
  q <-.-> r
```

### Arrow Length

Shorter arrows appear earlier than longer arrows...

```mermaid
flowchart LR
  a --- b
  c ---- d
  e === f
  g ==== h
  i -.-> j
  k -..-> l
```

## Edge Text

```mermaid
flowchart LR
  a ---|"edge text"|b
```

## Multiple Edges

### To the same node

```mermaid
flowchart LR
  a -->|"first"| b
  a -->|"second"| b
```

### Between multiple nodes

```mermaid
flowchart LR
  1 --> 2 & 3
  a --> b & c
  m & n --> p & q
```

## Styling

I won't expore this yet until I need it.

## Subgraphs

### Basic

```mermaid
flowchart LR
  a --> b
  subgraph subgraphId
    c --> d
  end
```

### Subgraph Text

```mermaid
flowchart LR
  a --> b
  subgraph subgraphId ["subgraph text"]
    c --> d
  end
```

### Subgraph Links

```mermaid
flowchart LR
  a --> b
  subgraph subgraphId ["subgraph text"]
    c --> d
  end
  b --> subgraphId
  a --> c
```

### Subgraph Direction

```mermaid
flowchart LR
  subgraph subgraphId1 ["TB"]
    direction TB
    a --> b
  end
  subgraph subgraphId2 ["BT"]
    direction BT
    c --> d
  end
  subgraph subgraphId3 ["LR"]
    direction LR
    e --> f
  end
  subgraph subgraphId4 ["RL"]
    direction RL
    g --> h
  end
```