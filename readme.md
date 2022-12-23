p100 crc bruteforce for [`tier1/checksum_crc.cpp`](https://github.com/ValveSoftware/source-sdk-2013/blob/master/sp/src/tier1/checksum_crc.cpp)

leaving this here for reuse in the future, maybe

```rust
const CRC_32_CSGO: Algorithm<u32> = Algorithm {
    width: 32,
    poly: 79764919,
    init: 0xffffffff,
    refin: true,
    refout: false,
    xorout: 0xffffffff,
    check: 0,
    residue: 0,
};

const CSGO: Crc<u32> = Crc::<u32>::new(&CRC_32_CSGO);
```
