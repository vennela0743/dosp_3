# dosp_3
# Chord Protocol Implementation in Pony

## Project Overview

This project, created by Sai Lakshmana Chandan Abhishek Muchukota and Vennela Priya Penumuchu, implements the Chord protocol in the Pony programming language. The goal is to demonstrate the effectiveness of Chord for distributed key-value lookup, using the Actor Model to represent each peer in a scalable and efficient manner.

## Features

- **Chord Protocol Implementation**: Supports node join, finger table management, and stabilization as described in the Chord protocol.
- **Pony Actor Model**: Uses actors to represent each peer, ensuring efficient concurrent message handling and fault tolerance.
- **Distributed Hash Table (DHT)**: Provides key-value association and lookup within the network, allowing each peer to store and retrieve values by key.
- **Network Simulation**: Simulates a network of peers and measures performance based on the average number of hops for message delivery.

## Project Structure

- **Peer Actor**: Implements the core functionality of each Chord node, including:
  - **Join Ring**: Allows new nodes to join the Chord ring.
  - **Find Successor**: Locates the node responsible for a given key.
  - **Stabilize**: Ensures the ring remains connected as peers join or leave.
  - **Fix Fingers**: Updates finger tables periodically for efficient routing.
- **Main Actor**: Initializes the network and runs the simulation by generating peers and testing message routing.


