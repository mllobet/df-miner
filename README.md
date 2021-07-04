# df-miner
Containerized mimc-fast miner setup backed with nginx

## Instructions

To run the miner
`docker compose up`

To test the miner
`curl --data '{"chunkFootprint": { "bottomLeft": { "x": 0, "y": 0 }, "sideLength": 256 }, "planetRarity":16384, "planetHashKey": 8}' -H "Content-Type: application/json" -X POST http://0.0.0.0:8001/mine`
