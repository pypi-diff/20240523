# Comparing `tmp/chia_rs-0.8.0.tar.gz` & `tmp/chia_rs-0.9.0.tar.gz`

## Comparing `chia_rs-0.8.0.tar` & `chia_rs-0.9.0.tar`

### file list

```diff
@@ -1,147 +1,153 @@
--rw-r--r--   0     1001      127     1213 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/Cargo.toml
--rw-r--r--   0     1001      127     7024 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/block_record.rs
--rw-r--r--   0     1001      127    17592 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/bytes.rs
--rw-r--r--   0     1001      127     5494 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/chia_protocol.rs
--rw-r--r--   0     1001      127     1194 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/classgroup.rs
--rw-r--r--   0     1001      127     4462 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/coin.rs
--rw-r--r--   0     1001      127      199 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      127      198 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/coin_state.rs
--rw-r--r--   0     1001      127      397 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      127      531 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      127     1983 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/foliage.rs
--rw-r--r--   0     1001      127     3492 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/full_node_protocol.rs
--rw-r--r--   0     1001      127     4342 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/fullblock.rs
--rw-r--r--   0     1001      127     4114 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/header_block.rs
--rw-r--r--   0     1001      127     1406 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/lazy_node.rs
--rw-r--r--   0     1001      127     1423 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/lib.rs
--rw-r--r--   0     1001      127      142 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/peer_info.rs
--rw-r--r--   0     1001      127      195 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/pool_target.rs
--rw-r--r--   0     1001      127    17486 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/program.rs
--rw-r--r--   0     1001      127      319 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      127     1967 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      127     1458 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/slots.rs
--rw-r--r--   0     1001      127     8244 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      127      449 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/sub_epoch_summary.rs
--rw-r--r--   0     1001      127     2343 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/unfinished_block.rs
--rw-r--r--   0     1001      127     1856 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/unfinished_header_block.rs
--rw-r--r--   0     1001      127      338 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/vdf.rs
--rw-r--r--   0     1001      127     6158 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      127     2361 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-protocol/src/weight_proof.rs
--rw-r--r--   0     1001      127      454 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127    16368 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia_py_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127     1365 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/Cargo.toml
--rw-r--r--   0     1001      127     2115 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/README.md
--rw-r--r--   0     1001      127     2797 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/benches/cache.rs
--rw-r--r--   0     1001      127     1389 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/benches/derive_key.rs
--rw-r--r--   0     1001      127     1356 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/benches/parse.rs
--rw-r--r--   0     1001      127      828 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/benches/sign.rs
--rw-r--r--   0     1001      127     2016 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/benches/verify.rs
--rw-r--r--   0     1001      127     8777 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/cached_bls.rs
--rw-r--r--   0     1001      127       78 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/derivable_key.rs
--rw-r--r--   0     1001      127     1500 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/derive_keys.rs
--rw-r--r--   0     1001      127     1114 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/error.rs
--rw-r--r--   0     1001      127     4619 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/gtelement.rs
--rw-r--r--   0     1001      127      636 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/lib.rs
--rw-r--r--   0     1001      127     4484 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/mnemonic.rs
--rw-r--r--   0     1001      127    26545 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/public_key.rs
--rw-r--r--   0     1001      127    19147 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/secret_key.rs
--rw-r--r--   0     1001      127    44458 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-bls/src/signature.rs
--rw-r--r--   0     1001      127      516 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127     9371 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127      548 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-utils/Cargo.toml
--rw-r--r--   0     1001      127     2069 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-utils/src/curried_program.rs
--rw-r--r--   0     1001      127     1909 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-utils/src/curry_tree_hash.rs
--rw-r--r--   0     1001      127     2624 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-utils/src/hash_encoder.rs
--rw-r--r--   0     1001      127      849 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-utils/src/lib.rs
--rw-r--r--   0     1001      127    10970 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-utils/src/tree_hash.rs
--rw-r--r--   0     1001      127      408 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-derive/Cargo.toml
--rw-r--r--   0     1001      127    10152 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-derive/src/from_clvm.rs
--rw-r--r--   0     1001      127     2602 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-derive/src/helpers.rs
--rw-r--r--   0     1001      127      603 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-derive/src/lib.rs
--rw-r--r--   0     1001      127     1217 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-derive/src/macros.rs
--rw-r--r--   0     1001      127     7548 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-derive/src/to_clvm.rs
--rw-r--r--   0     1001      127      468 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/Cargo.toml
--rw-r--r--   0     1001      127      839 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/src/chia_error.rs
--rw-r--r--   0     1001      127     2346 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/src/from_json_dict.rs
--rw-r--r--   0     1001      127     2484 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/src/int.rs
--rw-r--r--   0     1001      127      457 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/src/lib.rs
--rw-r--r--   0     1001      127    20419 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/src/streamable.rs
--rw-r--r--   0     1001      127     1892 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-traits/src/to_json_dict.rs
--rw-r--r--   0     1001      127     1521 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/Cargo.toml
--rw-r--r--   0     1001      127     4313 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/README.md
--rw-r--r--   0     1001      127     2274 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/benches/merkle-set.rs
--rw-r--r--   0     1001      127     3186 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/benches/run-generator.rs
--rw-r--r--   0     1001      127     2182 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/benches/tree-hash.rs
--rw-r--r--   0     1001      127      266 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/allocator.rs
--rw-r--r--   0     1001      127     4085 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/consensus_constants.rs
--rw-r--r--   0     1001      127     1370 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/error.rs
--rw-r--r--   0     1001      127    17402 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/fast_forward.rs
--rw-r--r--   0     1001      127     3068 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/coin_id.rs
--rw-r--r--   0     1001      127     5714 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      127   189253 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/conditions.rs
--rw-r--r--   0     1001      127     1751 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/flags.rs
--rw-r--r--   0     1001      127     6426 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      127     9647 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/messages.rs
--rw-r--r--   0     1001      127      506 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/mod.rs
--rw-r--r--   0     1001      127    11894 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/opcodes.rs
--rw-r--r--   0     1001      127     5466 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/owned_conditions.rs
--rw-r--r--   0     1001      127     6807 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      127     2004 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      127     2944 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      127    10868 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/solution_generator.rs
--rw-r--r--   0     1001      127      471 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/spend_visitor.rs
--rw-r--r--   0     1001      127     9411 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/test_generators.rs
--rw-r--r--   0     1001      127    14899 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/gen/validation_error.rs
--rw-r--r--   0     1001      127     3133 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/generator_rom.rs
--rw-r--r--   0     1001      127      202 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/lib.rs
--rw-r--r--   0     1001      127    17854 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/merkle_set.rs
--rw-r--r--   0     1001      127    32195 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-consensus/src/merkle_tree.rs
--rw-r--r--   0     1001      127      802 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/Cargo.toml
--rw-r--r--   0     1001      127     6968 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/docs/derive_macros.md
--rw-r--r--   0     1001      127     1742 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/clvm_decoder.rs
--rw-r--r--   0     1001      127     1518 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/clvm_encoder.rs
--rw-r--r--   0     1001      127     1067 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/error.rs
--rw-r--r--   0     1001      127    10932 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/from_clvm.rs
--rw-r--r--   0     1001      127     5612 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/lib.rs
--rw-r--r--   0     1001      127     3246 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/macros.rs
--rw-r--r--   0     1001      127     1026 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/match_byte.rs
--rw-r--r--   0     1001      127     8909 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/to_clvm.rs
--rw-r--r--   0     1001      127      670 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/clvm-traits/src/wrappers.rs
--rw-r--r--   0     1001      127      876 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/Cargo.toml
--rw-r--r--   0     1001      127     6407 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/derive_synthetic.rs
--rw-r--r--   0     1001      127      114 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/lib.rs
--rw-r--r--   0     1001      127      789 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/proof.rs
--rw-r--r--   0     1001      127    14594 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/cat.rs
--rw-r--r--   0     1001      127     4690 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/did.rs
--rw-r--r--   0     1001      127    14167 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/nft.rs
--rw-r--r--   0     1001      127     4011 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/offer.rs
--rw-r--r--   0     1001      127     5065 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/singleton.rs
--rw-r--r--   0     1001      127     3146 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/standard.rs
--rw-r--r--   0     1001      127      427 2024-05-14 21:11:23.000000 chia_rs-0.8.0/crates/chia-puzzles/src/puzzles.rs
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 chia_rs-0.8.0/wheel/Cargo.toml
--rw-r--r--   0     1001      127       78 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/README.md
--rw-r--r--   0     1001      127    16321 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/generate_type_stubs.py
--rw-r--r--   0     1001      127        0 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/py.typed
--rw-r--r--   0     1001      127       23 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/__init__.py
--rw-r--r--   0     1001      127   170298 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/chia_rs.pyi
--rw-r--r--   0     1001      127        0 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/py.typed
--rw-r--r--   0     1001      127     2708 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/sized_byte_class.py
--rw-r--r--   0     1001      127      385 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/sized_bytes.py
--rw-r--r--   0     1001      127     1629 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/sized_ints.py
--rw-r--r--   0     1001      127     3974 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/python/chia_rs/struct_stream.py
--rw-r--r--   0     1001      127      364 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/src/adapt_response.rs
--rw-r--r--   0     1001      127    19747 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/src/api.rs
--rw-r--r--   0     1001      127      158 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/src/lib.rs
--rw-r--r--   0     1001      127     3939 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/src/run_generator.rs
--rw-r--r--   0     1001      127     1788 2024-05-14 21:11:23.000000 chia_rs-0.8.0/wheel/src/run_program.rs
--rw-r--r--   0     1001      127    69312 2024-05-14 21:11:23.000000 chia_rs-0.8.0/Cargo.lock
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 chia_rs-0.8.0/Cargo.toml
--rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 chia_rs-0.8.0/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/py.typed
--rw-r--r--   0     1001      127   170298 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/chia_rs.pyi
--rw-r--r--   0     1001      127     3974 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/struct_stream.py
--rw-r--r--   0     1001      127      385 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/sized_bytes.py
--rw-r--r--   0     1001      127       23 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/__init__.py
--rw-r--r--   0     1001      127     1629 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/sized_ints.py
--rw-r--r--   0     1001      127     2708 2024-05-14 21:11:23.000000 chia_rs-0.8.0/python/chia_rs/sized_byte_class.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 chia_rs-0.8.0/PKG-INFO
+-rw-r--r--   0     1001      127     1519 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/Cargo.toml
+-rw-r--r--   0     1001      127     4313 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/README.md
+-rw-r--r--   0     1001      127     2274 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/benches/merkle-set.rs
+-rw-r--r--   0     1001      127     3186 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/benches/run-generator.rs
+-rw-r--r--   0     1001      127     2182 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/benches/tree-hash.rs
+-rw-r--r--   0     1001      127      266 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/allocator.rs
+-rw-r--r--   0     1001      127     6077 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/consensus_constants.rs
+-rw-r--r--   0     1001      127     1370 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/error.rs
+-rw-r--r--   0     1001      127    17402 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/fast_forward.rs
+-rw-r--r--   0     1001      127     3068 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/coin_id.rs
+-rw-r--r--   0     1001      127     5714 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      127   191877 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/conditions.rs
+-rw-r--r--   0     1001      127     2096 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/flags.rs
+-rw-r--r--   0     1001      127     6426 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      127     9647 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/messages.rs
+-rw-r--r--   0     1001      127      506 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/mod.rs
+-rw-r--r--   0     1001      127    11894 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/opcodes.rs
+-rw-r--r--   0     1001      127     5264 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/owned_conditions.rs
+-rw-r--r--   0     1001      127     6807 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      127     2004 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      127     2944 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      127    10868 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/solution_generator.rs
+-rw-r--r--   0     1001      127      471 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/spend_visitor.rs
+-rw-r--r--   0     1001      127     9313 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/test_generators.rs
+-rw-r--r--   0     1001      127    14899 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/gen/validation_error.rs
+-rw-r--r--   0     1001      127     3133 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/generator_rom.rs
+-rw-r--r--   0     1001      127      202 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/lib.rs
+-rw-r--r--   0     1001      127    17854 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/merkle_set.rs
+-rw-r--r--   0     1001      127    32214 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-consensus/src/merkle_tree.rs
+-rw-r--r--   0     1001      127      408 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/Cargo.toml
+-rw-r--r--   0     1001      127     1321 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/apply_constants.rs
+-rw-r--r--   0     1001      127    13655 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/from_clvm.rs
+-rw-r--r--   0     1001      127     2555 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/helpers.rs
+-rw-r--r--   0     1001      127     1039 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/lib.rs
+-rw-r--r--   0     1001      127     6625 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/parser/attributes.rs
+-rw-r--r--   0     1001      127     2240 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/parser/enum_info.rs
+-rw-r--r--   0     1001      127     2873 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/parser/field_info.rs
+-rw-r--r--   0     1001      127     1680 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/parser/struct_info.rs
+-rw-r--r--   0     1001      127     1703 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/parser/variant_info.rs
+-rw-r--r--   0     1001      127      703 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/parser.rs
+-rw-r--r--   0     1001      127    10010 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-derive/src/to_clvm.rs
+-rw-r--r--   0     1001      127      800 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/Cargo.toml
+-rw-r--r--   0     1001      127    11888 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/docs/derive_macros.md
+-rw-r--r--   0     1001      127     2243 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/clvm_decoder.rs
+-rw-r--r--   0     1001      127     1811 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/clvm_encoder.rs
+-rw-r--r--   0     1001      127     1067 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/error.rs
+-rw-r--r--   0     1001      127    10932 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/from_clvm.rs
+-rw-r--r--   0     1001      127     8335 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/lib.rs
+-rw-r--r--   0     1001      127     3246 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/macros.rs
+-rw-r--r--   0     1001      127     1026 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/match_byte.rs
+-rw-r--r--   0     1001      127     8909 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/to_clvm.rs
+-rw-r--r--   0     1001      127      670 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-traits/src/wrappers.rs
+-rw-r--r--   0     1001      127      548 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-utils/Cargo.toml
+-rw-r--r--   0     1001      127     2069 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-utils/src/curried_program.rs
+-rw-r--r--   0     1001      127     1909 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-utils/src/curry_tree_hash.rs
+-rw-r--r--   0     1001      127     2624 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-utils/src/hash_encoder.rs
+-rw-r--r--   0     1001      127      849 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-utils/src/lib.rs
+-rw-r--r--   0     1001      127    10970 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/clvm-utils/src/tree_hash.rs
+-rw-r--r--   0     1001      127      468 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/Cargo.toml
+-rw-r--r--   0     1001      127      839 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/src/chia_error.rs
+-rw-r--r--   0     1001      127     2436 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/src/from_json_dict.rs
+-rw-r--r--   0     1001      127     2513 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/src/int.rs
+-rw-r--r--   0     1001      127      457 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/src/lib.rs
+-rw-r--r--   0     1001      127    20419 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/src/streamable.rs
+-rw-r--r--   0     1001      127     1910 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-traits/src/to_json_dict.rs
+-rw-r--r--   0     1001      127      876 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/Cargo.toml
+-rw-r--r--   0     1001      127     6407 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/derive_synthetic.rs
+-rw-r--r--   0     1001      127      114 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/lib.rs
+-rw-r--r--   0     1001      127      785 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/proof.rs
+-rw-r--r--   0     1001      127    15168 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/cat.rs
+-rw-r--r--   0     1001      127     4690 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/did.rs
+-rw-r--r--   0     1001      127    17383 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/nft.rs
+-rw-r--r--   0     1001      127     4030 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/offer.rs
+-rw-r--r--   0     1001      127     5713 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/singleton.rs
+-rw-r--r--   0     1001      127     3699 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/standard.rs
+-rw-r--r--   0     1001      127      427 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-puzzles/src/puzzles.rs
+-rw-r--r--   0     1001      127     1365 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/Cargo.toml
+-rw-r--r--   0     1001      127     2115 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/README.md
+-rw-r--r--   0     1001      127     2763 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/benches/cache.rs
+-rw-r--r--   0     1001      127     1389 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/benches/derive_key.rs
+-rw-r--r--   0     1001      127     1356 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/benches/parse.rs
+-rw-r--r--   0     1001      127      828 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/benches/sign.rs
+-rw-r--r--   0     1001      127     2016 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/benches/verify.rs
+-rw-r--r--   0     1001      127     9064 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/cached_bls.rs
+-rw-r--r--   0     1001      127       78 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/derivable_key.rs
+-rw-r--r--   0     1001      127     1500 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/derive_keys.rs
+-rw-r--r--   0     1001      127     1114 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/error.rs
+-rw-r--r--   0     1001      127     4695 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/gtelement.rs
+-rw-r--r--   0     1001      127      636 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/lib.rs
+-rw-r--r--   0     1001      127     4484 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/mnemonic.rs
+-rw-r--r--   0     1001      127    27360 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/public_key.rs
+-rw-r--r--   0     1001      127    19162 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/secret_key.rs
+-rw-r--r--   0     1001      127    44473 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-bls/src/signature.rs
+-rw-r--r--   0     1001      127      516 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127     9371 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127      454 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127    16653 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia_py_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127     1213 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/Cargo.toml
+-rw-r--r--   0     1001      127     7193 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/block_record.rs
+-rw-r--r--   0     1001      127    18390 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/bytes.rs
+-rw-r--r--   0     1001      127     5550 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/chia_protocol.rs
+-rw-r--r--   0     1001      127     1194 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      127     4475 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/coin.rs
+-rw-r--r--   0     1001      127      199 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      127      198 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      127      397 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      127      531 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      127     1983 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/foliage.rs
+-rw-r--r--   0     1001      127     3492 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/full_node_protocol.rs
+-rw-r--r--   0     1001      127     4363 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      127     4135 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/header_block.rs
+-rw-r--r--   0     1001      127     1365 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/lazy_node.rs
+-rw-r--r--   0     1001      127     1423 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/lib.rs
+-rw-r--r--   0     1001      127      142 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/peer_info.rs
+-rw-r--r--   0     1001      127      195 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      127    17593 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/program.rs
+-rw-r--r--   0     1001      127      319 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      127     1967 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      127     1458 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/slots.rs
+-rw-r--r--   0     1001      127     8248 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      127      449 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/sub_epoch_summary.rs
+-rw-r--r--   0     1001      127     2350 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/unfinished_block.rs
+-rw-r--r--   0     1001      127     1863 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/unfinished_header_block.rs
+-rw-r--r--   0     1001      127      338 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/vdf.rs
+-rw-r--r--   0     1001      127     6175 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      127     2361 2024-05-23 21:03:07.000000 chia_rs-0.9.0/crates/chia-protocol/src/weight_proof.rs
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 chia_rs-0.9.0/wheel/Cargo.toml
+-rw-r--r--   0     1001      127       78 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/README.md
+-rw-r--r--   0     1001      127    16470 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/generate_type_stubs.py
+-rw-r--r--   0     1001      127        0 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/py.typed
+-rw-r--r--   0     1001      127       23 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/__init__.py
+-rw-r--r--   0     1001      127   170576 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/chia_rs.pyi
+-rw-r--r--   0     1001      127        0 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/py.typed
+-rw-r--r--   0     1001      127     2708 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/sized_byte_class.py
+-rw-r--r--   0     1001      127      385 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/sized_bytes.py
+-rw-r--r--   0     1001      127     1629 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/sized_ints.py
+-rw-r--r--   0     1001      127     3974 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/python/chia_rs/struct_stream.py
+-rw-r--r--   0     1001      127      364 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/src/adapt_response.rs
+-rw-r--r--   0     1001      127    20105 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/src/api.rs
+-rw-r--r--   0     1001      127      158 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/src/lib.rs
+-rw-r--r--   0     1001      127     3953 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/src/run_generator.rs
+-rw-r--r--   0     1001      127     1788 2024-05-23 21:03:07.000000 chia_rs-0.9.0/wheel/src/run_program.rs
+-rw-r--r--   0     1001      127    69759 2024-05-23 21:03:07.000000 chia_rs-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 chia_rs-0.9.0/Cargo.toml
+-rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 chia_rs-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      127   170576 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/chia_rs.pyi
+-rw-r--r--   0     1001      127     1629 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/sized_ints.py
+-rw-r--r--   0     1001      127       23 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/py.typed
+-rw-r--r--   0     1001      127     2708 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/sized_byte_class.py
+-rw-r--r--   0     1001      127      385 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/sized_bytes.py
+-rw-r--r--   0     1001      127     3974 2024-05-23 21:03:07.000000 chia_rs-0.9.0/python/chia_rs/struct_stream.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 chia_rs-0.9.0/PKG-INFO
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/Cargo.toml` & `chia_rs-0.9.0/crates/chia-protocol/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [package]
 name = "chia-protocol"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chia network protocol message types"
 authors = ["Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chia_py_streamable_macro", "chia-traits/py-bindings", "chia-bls/py-bindings"]
 arbitrary = ["dep:arbitrary", "chia-bls/arbitrary"]
 
 [dependencies]
-pyo3 = { version = "0.19.0", features = ["multiple-pymethods", "num-bigint"], optional = true }
+pyo3 = { version = "0.21.2", features = ["multiple-pymethods", "num-bigint"], optional = true }
 sha2 = "0.10.8"
 hex = "0.4.3"
 chia_streamable_macro = { version = "0.8.0", path = "../chia_streamable_macro" }
-chia_py_streamable_macro = { version = "0.7.0", path = "../chia_py_streamable_macro", optional = true }
+chia_py_streamable_macro = { version = "0.9.0", path = "../chia_py_streamable_macro", optional = true }
 clvmr = "0.7.0"
-chia-traits = { version = "0.8.0", path = "../chia-traits" }
-clvm-traits = { version = "0.8.0", path = "../clvm-traits", features = ["derive"] }
-clvm-utils = { version = "0.8.0", path = "../clvm-utils" }
-chia-bls = { version = "0.8.0", path = "../chia-bls" }
+chia-traits = { version = "0.9.0", path = "../chia-traits" }
+clvm-traits = { version = "0.9.0", path = "../clvm-traits", features = ["derive"] }
+clvm-utils = { version = "0.9.0", path = "../clvm-utils" }
+chia-bls = { version = "0.9.0", path = "../chia-bls" }
 arbitrary = { version = "1.3.0", features = ["derive"], optional = true }
 
 [dev-dependencies]
 rstest = "0.17.0"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/block_record.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/block_record.rs`

 * *Files 6% similar despite different names*

```diff
@@ -90,99 +90,103 @@
     #[getter]
     #[pyo3(name = "first_in_sub_slot")]
     fn py_first_in_sub_slot(&self) -> bool {
         self.first_in_sub_slot()
     }
 
     #[pyo3(name = "is_challenge_block")]
-    fn py_is_challenge_block(&self, constants: &PyAny) -> PyResult<bool> {
+    fn py_is_challenge_block(&self, constants: &Bound<PyAny>) -> PyResult<bool> {
         Ok(self.is_challenge_block(
             constants
                 .getattr("MIN_BLOCKS_PER_CHALLENGE_BLOCK")?
                 .extract::<u8>()?,
         ))
     }
 
     // TODO: at some point it would be nice to port
     // chia.consensus.pot_iterations to rust, and make this less hacky
-    fn sp_sub_slot_total_iters_impl(&self, py: Python, constants: &PyAny) -> PyResult<u128> {
+    fn sp_sub_slot_total_iters_impl(&self, py: Python, constants: &Bound<PyAny>) -> PyResult<u128> {
         let ret = self
             .total_iters
             .checked_sub(self.ip_iters_impl(py, constants)? as u128)
             .ok_or(PyValueError::new_err("uint128 overflow"))?;
         if self.overflow {
             ret.checked_sub(self.sub_slot_iters as u128)
                 .ok_or(PyValueError::new_err("uint128 overflow"))
         } else {
             Ok(ret)
         }
     }
 
-    fn ip_sub_slot_total_iters_impl(&self, py: Python, constants: &PyAny) -> PyResult<u128> {
+    fn ip_sub_slot_total_iters_impl(&self, py: Python, constants: &Bound<PyAny>) -> PyResult<u128> {
         self.total_iters
             .checked_sub(self.ip_iters_impl(py, constants)? as u128)
             .ok_or(PyValueError::new_err("uint128 overflow"))
     }
 
-    fn sp_iters_impl(&self, py: Python, constants: &PyAny) -> PyResult<u64> {
-        let ctx: &PyDict = PyDict::new(py);
+    fn sp_iters_impl(&self, py: Python, constants: &Bound<PyAny>) -> PyResult<u64> {
+        let ctx = PyDict::new_bound(py);
         ctx.set_item("sub_slot_iters", self.sub_slot_iters)?;
         ctx.set_item("signage_point_index", self.signage_point_index)?;
         ctx.set_item("constants", constants)?;
-        py.run(
+        py.run_bound(
             "from chia.consensus.pot_iterations import calculate_ip_iters, calculate_sp_iters\n\
             ret = calculate_sp_iters(constants, sub_slot_iters, signage_point_index)\n",
             None,
-            Some(ctx),
+            Some(&ctx),
         )?;
-        ctx.get_item("ret").unwrap().extract::<u64>()
+        ctx.get_item("ret").unwrap().unwrap().extract::<u64>()
     }
 
-    fn ip_iters_impl(&self, py: Python, constants: &PyAny) -> PyResult<u64> {
-        let ctx: &PyDict = PyDict::new(py);
+    fn ip_iters_impl(&self, py: Python, constants: &Bound<PyAny>) -> PyResult<u64> {
+        let ctx = PyDict::new_bound(py);
         ctx.set_item("sub_slot_iters", self.sub_slot_iters)?;
         ctx.set_item("signage_point_index", self.signage_point_index)?;
         ctx.set_item("required_iters", self.required_iters)?;
         ctx.set_item("constants", constants)?;
-        py.run(
+        py.run_bound(
             "from chia.consensus.pot_iterations import calculate_ip_iters, calculate_sp_iters\n\
             ret = calculate_ip_iters(constants, sub_slot_iters, signage_point_index, required_iters)\n",
             None,
-            Some(ctx),
+            Some(&ctx),
             )?;
-        ctx.get_item("ret").unwrap().extract::<u64>()
+        ctx.get_item("ret").unwrap().unwrap().extract::<u64>()
     }
 
-    fn sp_total_iters_impl(&self, py: Python, constants: &PyAny) -> PyResult<u128> {
+    fn sp_total_iters_impl(&self, py: Python, constants: &Bound<PyAny>) -> PyResult<u128> {
         self.sp_sub_slot_total_iters_impl(py, constants)?
             .checked_add(self.sp_iters_impl(py, constants)? as u128)
             .ok_or(PyValueError::new_err("uint128 overflow"))
     }
 
     fn sp_sub_slot_total_iters<'a>(
         &self,
         py: Python<'a>,
-        constants: &PyAny,
-    ) -> PyResult<&'a PyAny> {
+        constants: &Bound<PyAny>,
+    ) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.sp_sub_slot_total_iters_impl(py, constants)?, py)
     }
 
     fn ip_sub_slot_total_iters<'a>(
         &self,
         py: Python<'a>,
-        constants: &PyAny,
-    ) -> PyResult<&'a PyAny> {
+        constants: &Bound<PyAny>,
+    ) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.ip_sub_slot_total_iters_impl(py, constants)?, py)
     }
 
-    fn sp_iters<'a>(&self, py: Python<'a>, constants: &PyAny) -> PyResult<&'a PyAny> {
+    fn sp_iters<'a>(&self, py: Python<'a>, constants: &Bound<PyAny>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.sp_iters_impl(py, constants)?, py)
     }
 
-    fn ip_iters<'a>(&self, py: Python<'a>, constants: &PyAny) -> PyResult<&'a PyAny> {
+    fn ip_iters<'a>(&self, py: Python<'a>, constants: &Bound<PyAny>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.ip_iters_impl(py, constants)?, py)
     }
 
-    fn sp_total_iters<'a>(&self, py: Python<'a>, constants: &PyAny) -> PyResult<&'a PyAny> {
+    fn sp_total_iters<'a>(
+        &self,
+        py: Python<'a>,
+        constants: &Bound<PyAny>,
+    ) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.sp_total_iters_impl(py, constants)?, py)
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/bytes.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/bytes.rs`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         self.0.is_empty()
     }
 
     pub fn as_slice(&self) -> &[u8] {
         self.0.as_slice()
     }
 
+    pub fn to_vec(&self) -> Vec<u8> {
+        self.0.clone()
+    }
+
     pub fn into_inner(self) -> Vec<u8> {
         self.0
     }
 }
 
 impl fmt::Debug for Bytes {
     fn fmt(&self, formatter: &mut fmt::Formatter<'_>) -> fmt::Result {
@@ -83,15 +87,15 @@
     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
         Ok(format!("0x{self}").to_object(py))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl FromJsonDict for Bytes {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         let s: String = o.extract()?;
         if !s.starts_with("0x") {
             return Err(PyValueError::new_err(
                 "bytes object is expected to start with 0x",
             ));
         }
         let s = &s[2..];
@@ -120,14 +124,20 @@
 
 impl From<&[u8]> for Bytes {
     fn from(value: &[u8]) -> Self {
         Self(value.to_vec())
     }
 }
 
+impl<const N: usize> From<BytesImpl<N>> for Bytes {
+    fn from(value: BytesImpl<N>) -> Self {
+        Self(value.0.to_vec())
+    }
+}
+
 impl From<Vec<u8>> for Bytes {
     fn from(value: Vec<u8>) -> Self {
         Self(value)
     }
 }
 
 impl From<Bytes> for Vec<u8> {
@@ -151,18 +161,26 @@
 }
 
 #[derive(Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Hash)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 pub struct BytesImpl<const N: usize>([u8; N]);
 
 impl<const N: usize> BytesImpl<N> {
-    pub fn new(bytes: [u8; N]) -> Self {
+    pub const fn new(bytes: [u8; N]) -> Self {
         Self(bytes)
     }
 
+    pub const fn len(&self) -> usize {
+        N
+    }
+
+    pub const fn is_empty(&self) -> bool {
+        N == 0
+    }
+
     pub fn as_slice(&self) -> &[u8] {
         &self.0
     }
 
     pub fn to_bytes(self) -> [u8; N] {
         self.0
     }
@@ -209,15 +227,15 @@
     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
         Ok(format!("0x{self}").to_object(py))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> FromJsonDict for BytesImpl<N> {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         let s: String = o.extract()?;
         if !s.starts_with("0x") {
             return Err(PyValueError::new_err(
                 "bytes object is expected to start with 0x",
             ));
         }
         let s = &s[2..];
@@ -277,14 +295,30 @@
     type Error = TryFromSliceError;
 
     fn try_from(value: &Vec<u8>) -> Result<Self, TryFromSliceError> {
         value.as_slice().try_into()
     }
 }
 
+impl<const N: usize> TryFrom<Bytes> for BytesImpl<N> {
+    type Error = TryFromSliceError;
+
+    fn try_from(value: Bytes) -> Result<Self, TryFromSliceError> {
+        value.0.as_slice().try_into()
+    }
+}
+
+impl<const N: usize> TryFrom<&Bytes> for BytesImpl<N> {
+    type Error = TryFromSliceError;
+
+    fn try_from(value: &Bytes) -> Result<Self, TryFromSliceError> {
+        value.0.as_slice().try_into()
+    }
+}
+
 impl<const N: usize> From<BytesImpl<N>> for Vec<u8> {
     fn from(value: BytesImpl<N>) -> Self {
         value.to_vec()
     }
 }
 
 impl<const N: usize> From<[u8; N]> for BytesImpl<N> {
@@ -353,73 +387,73 @@
         Self(value.to_bytes())
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> ToPyObject for BytesImpl<N> {
     fn to_object(&self, py: Python) -> PyObject {
-        PyBytes::new(py, &self.0).into()
+        PyBytes::new_bound(py, &self.0).into()
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> IntoPy<PyObject> for BytesImpl<N> {
     fn into_py(self, py: Python) -> PyObject {
-        PyBytes::new(py, &self.0).into()
+        PyBytes::new_bound(py, &self.0).into()
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> ChiaToPython for BytesImpl<N> {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         if N == 32 {
-            let bytes_module = PyModule::import(py, "chia_rs.sized_bytes")?;
+            let bytes_module = PyModule::import_bound(py, "chia_rs.sized_bytes")?;
             let ty = bytes_module.getattr("bytes32")?;
             ty.call1((self.0.into_py(py),))
         } else {
-            Ok(PyBytes::new(py, &self.0).into())
+            Ok(PyBytes::new_bound(py, &self.0).into_any())
         }
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<'py, const N: usize> FromPyObject<'py> for BytesImpl<N> {
     fn extract(obj: &'py PyAny) -> PyResult<Self> {
-        let b = <PyBytes as PyTryFrom>::try_from(obj)?;
+        let b = obj.downcast::<PyBytes>()?;
         let slice: &[u8] = b.as_bytes();
         let buf: [u8; N] = slice.try_into()?;
         Ok(BytesImpl::<N>(buf))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl ToPyObject for Bytes {
     fn to_object(&self, py: Python) -> PyObject {
-        PyBytes::new(py, &self.0).into()
+        PyBytes::new_bound(py, &self.0).into()
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl IntoPy<PyObject> for Bytes {
     fn into_py(self, py: Python) -> PyObject {
-        PyBytes::new(py, &self.0).into()
+        PyBytes::new_bound(py, &self.0).into()
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl ChiaToPython for Bytes {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        Ok(PyBytes::new(py, &self.0).into())
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(PyBytes::new_bound(py, &self.0).into_any())
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<'py> FromPyObject<'py> for Bytes {
     fn extract(obj: &'py PyAny) -> PyResult<Self> {
-        let b = <PyBytes as PyTryFrom>::try_from(obj)?;
+        let b = obj.downcast::<PyBytes>()?;
         Ok(Bytes(b.as_bytes().to_vec()))
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/chia_protocol.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/chia_protocol.rs`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,16 @@
     RequestCoinState = 101,
     RespondCoinState = 102,
     RejectCoinState = 103,
 }
 
 #[cfg(feature = "py-bindings")]
 impl chia_traits::ChiaToPython for ProtocolMessageTypes {
-    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
-        Ok(pyo3::IntoPy::into_py(*self, py).into_ref(py))
+    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<pyo3::Bound<'a, pyo3::PyAny>> {
+        Ok(pyo3::IntoPy::into_py(*self, py).bind(py).clone().into_any())
     }
 }
 
 pub trait ChiaProtocolMessage {
     fn msg_type() -> ProtocolMessageTypes;
 }
 
@@ -160,16 +160,16 @@
     Introducer = 5,
     Wallet = 6,
     DataLayer = 7,
 }
 
 #[cfg(feature = "py-bindings")]
 impl chia_traits::ChiaToPython for NodeType {
-    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
-        Ok(pyo3::IntoPy::into_py(*self, py).into_ref(py))
+    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<pyo3::Bound<'a, pyo3::PyAny>> {
+        Ok(pyo3::IntoPy::into_py(*self, py).bind(py).clone().into_any())
     }
 }
 
 #[streamable]
 pub struct Message {
     msg_type: ProtocolMessageTypes,
     id: Option<u16>,
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/classgroup.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/classgroup.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/coin.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/coin.rs`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         Bytes32::new(coin_id)
     }
 }
 
 #[cfg(feature = "py-bindings")]
 #[pymethods]
 impl Coin {
-    fn name<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
-        Ok(pyo3::types::PyBytes::new(py, &self.coin_id()))
+    fn name<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<Bound<'p, pyo3::types::PyBytes>> {
+        Ok(pyo3::types::PyBytes::new_bound(py, &self.coin_id()))
     }
 }
 
 impl<N> ToClvm<N> for Coin {
     fn to_clvm(&self, encoder: &mut impl ClvmEncoder<Node = N>) -> Result<N, ToClvmError> {
         clvm_list!(self.parent_coin_info, self.puzzle_hash, self.amount).to_clvm(encoder)
     }
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/fee_estimate.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/fee_estimate.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/foliage.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/foliage.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/full_node_protocol.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/full_node_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/fullblock.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/fullblock.rs`

 * *Files 5% similar despite different names*

```diff
@@ -108,27 +108,27 @@
     #[pyo3(name = "is_transaction_block")]
     fn py_is_transaction_block(&self) -> bool {
         self.is_transaction_block()
     }
 
     #[getter]
     #[pyo3(name = "total_iters")]
-    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.total_iters(), py)
     }
 
     #[getter]
     #[pyo3(name = "height")]
-    fn py_height<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_height<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.height(), py)
     }
 
     #[getter]
     #[pyo3(name = "weight")]
-    fn py_weight<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_weight<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.weight(), py)
     }
 
     #[pyo3(name = "get_included_reward_coins")]
     fn py_get_included_reward_coins(&self) -> Vec<Coin> {
         self.get_included_reward_coins()
     }
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/header_block.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/header_block.rs`

 * *Files 6% similar despite different names*

```diff
@@ -105,33 +105,33 @@
     #[pyo3(name = "prev_hash")]
     fn py_prev_hash(&self) -> Bytes32 {
         self.prev_hash()
     }
 
     #[getter]
     #[pyo3(name = "height")]
-    fn py_height<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_height<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.height(), py)
     }
 
     #[getter]
     #[pyo3(name = "weight")]
-    fn py_weight<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_weight<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.weight(), py)
     }
 
     #[getter]
     #[pyo3(name = "header_hash")]
     fn py_header_hash(&self) -> Bytes32 {
         self.header_hash()
     }
 
     #[getter]
     #[pyo3(name = "total_iters")]
-    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.total_iters(), py)
     }
 
     #[getter]
     #[pyo3(name = "log_string")]
     fn py_log_string(&self) -> String {
         self.log_string()
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/lazy_node.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/lazy_node.rs`

 * *Files 13% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 pub struct LazyNode {
     allocator: Rc<Allocator>,
     node: NodePtr,
 }
 
 impl ToPyObject for LazyNode {
     fn to_object(&self, py: Python<'_>) -> PyObject {
-        let node: &PyCell<LazyNode> = PyCell::new(py, self.clone()).unwrap();
-        let pa: &PyAny = node;
-        pa.to_object(py)
+        Bound::new(py, self.clone()).unwrap().to_object(py)
     }
 }
 
 #[pymethods]
 impl LazyNode {
     #[getter(pair)]
     pub fn pair(&self, py: Python) -> PyResult<Option<PyObject>> {
         match &self.allocator.sexp(self.node) {
             SExp::Pair(p1, p2) => {
                 let r1 = Self::new(self.allocator.clone(), *p1);
                 let r2 = Self::new(self.allocator.clone(), *p2);
-                let v: &PyTuple = PyTuple::new(py, &[r1, r2]);
+                let v = PyTuple::new_bound(py, &[r1, r2]);
                 Ok(Some(v.into()))
             }
             _ => Ok(None),
         }
     }
 
     #[getter(atom)]
     pub fn atom(&self, py: Python) -> Option<PyObject> {
         match &self.allocator.sexp(self.node) {
-            SExp::Atom => Some(PyBytes::new(py, self.allocator.atom(self.node).as_ref()).into()),
+            SExp::Atom => {
+                Some(PyBytes::new_bound(py, self.allocator.atom(self.node).as_ref()).into())
+            }
             _ => None,
         }
     }
 }
 
 impl LazyNode {
     pub const fn new(a: Rc<Allocator>, n: NodePtr) -> Self {
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/lib.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/program.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/program.rs`

 * *Files 3% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
 // TODO: this conversion function should probably be converted to a type holding
 // the PyAny object implementing the ToClvm trait. That way, the Program::to()
 // function could turn a python structure directly into bytes, without taking
 // the detour via Allocator. propagating python errors through ToClvmError is a
 // bit tricky though
 #[cfg(feature = "py-bindings")]
-fn clvm_convert(a: &mut Allocator, o: &PyAny) -> PyResult<NodePtr> {
+fn clvm_convert(a: &mut Allocator, o: &Bound<PyAny>) -> PyResult<NodePtr> {
     // None
     if o.is_none() {
         Ok(a.nil())
     // bytes
     } else if let Ok(buffer) = o.extract::<&[u8]>() {
         a.new_atom(buffer)
             .map_err(|e| PyMemoryError::new_err(e.to_string()))
@@ -190,42 +190,42 @@
     } else if let Ok(pair) = o.downcast::<PyTuple>() {
         if pair.len() != 2 {
             Err(PyValueError::new_err(format!(
                 "can't cast tuple of size {}",
                 pair.len()
             )))
         } else {
-            let left = clvm_convert(a, pair.get_item(0)?)?;
-            let right = clvm_convert(a, pair.get_item(1)?)?;
+            let left = clvm_convert(a, &pair.get_item(0)?)?;
+            let right = clvm_convert(a, &pair.get_item(1)?)?;
             a.new_pair(left, right)
                 .map_err(|e| PyMemoryError::new_err(e.to_string()))
         }
     // List
     } else if let Ok(list) = o.downcast::<PyList>() {
-        let mut rev = Vec::<&PyAny>::new();
+        let mut rev = Vec::new();
         for py_item in list.iter() {
             rev.push(py_item);
         }
         let mut ret = a.nil();
         for py_item in rev.into_iter().rev() {
-            let item = clvm_convert(a, py_item)?;
+            let item = clvm_convert(a, &py_item)?;
             ret = a
                 .new_pair(item, ret)
                 .map_err(|e| PyMemoryError::new_err(e.to_string()))?;
         }
         Ok(ret)
     // SExp (such as clvm.SExp)
     } else if let (Ok(atom), Ok(pair)) = (o.getattr("atom"), o.getattr("pair")) {
         if atom.is_none() {
             if pair.is_none() {
                 Err(PyTypeError::new_err(format!("invalid SExp item {o}")))
             } else {
                 let pair = pair.downcast::<PyTuple>()?;
-                let left = clvm_convert(a, &pair[0])?;
-                let right = clvm_convert(a, &pair[1])?;
+                let left = clvm_convert(a, &pair.get_item(0)?)?;
+                let right = clvm_convert(a, &pair.get_item(1)?)?;
                 a.new_pair(left, right)
                     .map_err(|e| PyMemoryError::new_err(e.to_string()))
             }
         } else {
             a.new_atom(atom.extract::<&[u8]>()?)
                 .map_err(|e| PyMemoryError::new_err(e.to_string()))
         }
@@ -245,15 +245,15 @@
         Err(PyTypeError::new_err(format!(
             "unknown parameter to run_with_cost() {o}"
         )))
     }
 }
 
 #[cfg(feature = "py-bindings")]
-fn clvm_serialize(a: &mut Allocator, o: &PyAny) -> PyResult<NodePtr> {
+fn clvm_serialize(a: &mut Allocator, o: &Bound<PyAny>) -> PyResult<NodePtr> {
     /*
     When passing arguments to run(), there's some special treatment, before falling
     back on the regular python -> CLVM conversion (implemented by clvm_convert
     above). This function mimics the _serialize() function in python:
 
        def _serialize(node: object) -> bytes:
            if isinstance(node, list):
@@ -270,37 +270,37 @@
            else:
                ret: bytes = SExp.to(node).as_bin()
                return ret
     */
 
     // List
     if let Ok(list) = o.downcast::<PyList>() {
-        let mut rev = Vec::<&PyAny>::new();
+        let mut rev = Vec::new();
         for py_item in list.iter() {
             rev.push(py_item);
         }
         let mut ret = a.nil();
         for py_item in rev.into_iter().rev() {
-            let item = clvm_serialize(a, py_item)?;
+            let item = clvm_serialize(a, &py_item)?;
             ret = a
                 .new_pair(item, ret)
                 .map_err(|e| PyMemoryError::new_err(e.to_string()))?;
         }
         Ok(ret)
     // Program itself
     } else if let Ok(prg) = o.extract::<Program>() {
         Ok(node_from_bytes_backrefs(a, prg.0.as_slice())?)
     } else {
         clvm_convert(a, o)
     }
 }
 
 #[cfg(feature = "py-bindings")]
-fn to_program(py: Python<'_>, node: LazyNode) -> PyResult<&PyAny> {
-    let int_module = PyModule::import(py, "chia.types.blockchain_format.program")?;
+fn to_program(py: Python<'_>, node: LazyNode) -> PyResult<Bound<PyAny>> {
+    let int_module = PyModule::import_bound(py, "chia.types.blockchain_format.program")?;
     let ty = int_module.getattr("Program")?;
     ty.call1((node.into_py(py),))
 }
 
 #[cfg(feature = "py-bindings")]
 #[pymethods]
 impl Program {
@@ -308,15 +308,15 @@
     #[staticmethod]
     fn py_default() -> Self {
         Self::default()
     }
 
     #[staticmethod]
     #[pyo3(name = "to")]
-    fn py_to(args: &PyAny) -> PyResult<Program> {
+    fn py_to(args: &Bound<PyAny>) -> PyResult<Program> {
         let mut a = Allocator::new_limited(500000000);
         let clvm = clvm_convert(&mut a, args)?;
         Program::from_node_ptr(&a, clvm)
             .map_err(|error| PyErr::new::<PyTypeError, _>(error.to_string()))
     }
 
     fn get_tree_hash(&self) -> crate::Bytes32 {
@@ -342,36 +342,36 @@
         Self::from_bytes(hex::decode(s).map_err(|_| Error::InvalidString)?.as_slice())
     }
 
     fn run_mempool_with_cost<'a>(
         &self,
         py: Python<'a>,
         max_cost: u64,
-        args: &PyAny,
-    ) -> PyResult<(u64, &'a PyAny)> {
+        args: &Bound<PyAny>,
+    ) -> PyResult<(u64, Bound<'a, PyAny>)> {
         use clvmr::MEMPOOL_MODE;
         self._run(py, max_cost, MEMPOOL_MODE, args)
     }
 
     fn run_with_cost<'a>(
         &self,
         py: Python<'a>,
         max_cost: u64,
-        args: &PyAny,
-    ) -> PyResult<(u64, &'a PyAny)> {
+        args: &Bound<PyAny>,
+    ) -> PyResult<(u64, Bound<'a, PyAny>)> {
         self._run(py, max_cost, 0, args)
     }
 
     fn _run<'a>(
         &self,
         py: Python<'a>,
         max_cost: u64,
         flags: u32,
-        args: &PyAny,
-    ) -> PyResult<(u64, &'a PyAny)> {
+        args: &Bound<PyAny>,
+    ) -> PyResult<(u64, Bound<'a, PyAny>)> {
         use clvmr::reduction::Response;
         use std::rc::Rc;
 
         let mut a = Allocator::new_limited(500000000);
         // The python behavior here is a bit messy, and is best not emulated
         // on the rust side. We must be able to pass a Program as an argument,
         // and it being treated as the CLVM structure it represents. In python's
@@ -397,23 +397,23 @@
             Err(eval_err) => {
                 let blob = node_to_bytes(&a, eval_err.0).ok().map(hex::encode);
                 Err(PyValueError::new_err((eval_err.1, blob)))
             }
         }
     }
 
-    fn to_program<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn to_program<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         use std::rc::Rc;
         let mut a = Allocator::new_limited(500000000);
         let prg = node_from_bytes_backrefs(&mut a, self.0.as_ref())?;
         let prg = LazyNode::new(Rc::new(a), prg);
         to_program(py, prg)
     }
 
-    fn uncurry<'a>(&self, py: Python<'a>) -> PyResult<(&'a PyAny, &'a PyAny)> {
+    fn uncurry<'a>(&self, py: Python<'a>) -> PyResult<(Bound<'a, PyAny>, Bound<'a, PyAny>)> {
         use clvm_utils::CurriedProgram;
         use std::rc::Rc;
 
         let mut a = Allocator::new_limited(500000000);
         let prg = node_from_bytes_backrefs(&mut a, self.0.as_ref())?;
         let Ok(uncurried) = CurriedProgram::<NodePtr, NodePtr>::from_node_ptr(&a, prg) else {
             let a = Rc::new(a);
@@ -483,15 +483,15 @@
     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
         self.0.to_json_dict(py)
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl FromJsonDict for Program {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         let bytes = Bytes::from_json_dict(o)?;
         let len =
             serialized_length_from_bytes(bytes.as_slice()).map_err(|_e| Error::EndOfBuffer)?;
         if len as usize != bytes.len() {
             // If the bytes in the JSON string is not a valid CLVM
             // serialization, or if it has garbage at the end of the string,
             // reject it
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/reward_chain_block.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/reward_chain_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/slots.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/slots.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/spend_bundle.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/spend_bundle.rs`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,21 @@
     fn py_additions(&self) -> PyResult<Vec<Coin>> {
         self.additions()
             .map_err(|e| pyo3::exceptions::PyValueError::new_err(e.1))
     }
 
     fn debug(&self, py: Python<'_>) -> PyResult<()> {
         use pyo3::types::PyDict;
-        let ctx: &PyDict = PyDict::new(py);
+        let ctx = PyDict::new_bound(py);
         ctx.set_item("self", self.clone().into_py(py))?;
-        py.run(
+        py.run_bound(
             "from chia.wallet.util.debug_spend_bundle import debug_spend_bundle\n\
             debug_spend_bundle(self)\n",
             None,
-            Some(ctx),
+            Some(&ctx),
         )
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/unfinished_block.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/unfinished_block.rs`

 * *Files 2% similar despite different names*

```diff
@@ -63,11 +63,11 @@
     #[pyo3(name = "is_transaction_block")]
     fn py_is_transaction_block(&self) -> bool {
         self.is_transaction_block()
     }
 
     #[getter]
     #[pyo3(name = "total_iters")]
-    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.total_iters(), py)
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/unfinished_header_block.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/unfinished_header_block.rs`

 * *Files 5% similar despite different names*

```diff
@@ -64,11 +64,11 @@
     #[pyo3(name = "header_hash")]
     fn py_header_hash(&self) -> Bytes32 {
         self.header_hash()
     }
 
     #[getter]
     #[pyo3(name = "total_iters")]
-    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn py_total_iters<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&self.total_iters(), py)
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/wallet_protocol.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/wallet_protocol.rs`

 * *Files 1% similar despite different names*

```diff
@@ -295,11 +295,11 @@
 pub enum RejectStateReason {
     Reorg = 0,
     ExceededSubscriptionLimit = 1,
 }
 
 #[cfg(feature = "py-bindings")]
 impl chia_traits::ChiaToPython for RejectStateReason {
-    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
-        Ok(pyo3::IntoPy::into_py(*self, py).into_ref(py))
+    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<pyo3::Bound<'a, pyo3::PyAny>> {
+        Ok(pyo3::IntoPy::into_py(*self, py).bind(py).clone())
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-protocol/src/weight_proof.rs` & `chia_rs-0.9.0/crates/chia-protocol/src/weight_proof.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia_py_streamable_macro/src/lib.rs` & `chia_rs-0.9.0/crates/chia_py_streamable_macro/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -93,16 +93,16 @@
                 let mut hasher = std::collections::hash_map::DefaultHasher::new();
                 std::hash::Hash::hash(self, &mut hasher);
                 Ok(std::hash::Hasher::finish(&hasher) as isize)
             }
         }
 
         impl #crate_name::ChiaToPython for #ident {
-            fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
-                Ok(pyo3::IntoPy::into_py(self.clone(), py).into_ref(py))
+            fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<pyo3::Bound<'a, pyo3::PyAny>> {
+                Ok(pyo3::IntoPy::into_py(self.clone(), py).into_bound(py))
             }
         }
     };
 
     let mut fnames = Vec::<syn::Ident>::new();
     let mut ftypes = Vec::<syn::Type>::new();
 
@@ -157,15 +157,15 @@
     }
 
     py_protocol.extend(quote! {
         #[pyo3::pymethods]
         impl #ident {
             #[staticmethod]
             #[pyo3(signature=(json_dict))]
-            pub fn from_json_dict(json_dict: &pyo3::PyAny) -> pyo3::PyResult<Self> {
+            pub fn from_json_dict(json_dict: &pyo3::Bound<pyo3::PyAny>) -> pyo3::PyResult<Self> {
                 <Self as #crate_name::from_json_dict::FromJsonDict>::from_json_dict(json_dict)
             }
 
             pub fn to_json_dict(&self, py: pyo3::Python) -> pyo3::PyResult<pyo3::PyObject> {
                 #crate_name::to_json_dict::ToJsonDict::to_json_dict(self, py)
             }
         }
@@ -212,31 +212,31 @@
                 if trusted {
                     <Self as #crate_name::Streamable>::parse::<true>(&mut input).map_err(|e| <#crate_name::chia_error::Error as Into<pyo3::PyErr>>::into(e)).map(|v| (v, input.position() as u32))
                 } else {
                     <Self as #crate_name::Streamable>::parse::<false>(&mut input).map_err(|e| <#crate_name::chia_error::Error as Into<pyo3::PyErr>>::into(e)).map(|v| (v, input.position() as u32))
                 }
             }
 
-            pub fn get_hash<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
+            pub fn get_hash<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<pyo3::Bound<'p, pyo3::types::PyBytes>> {
                 let mut ctx = <sha2::Sha256 as sha2::Digest>::new();
                 #crate_name::Streamable::update_digest(self, &mut ctx);
-                Ok(pyo3::types::PyBytes::new(py, sha2::Digest::finalize(ctx).as_slice()))
+                Ok(pyo3::types::PyBytes::new_bound(py, sha2::Digest::finalize(ctx).as_slice()))
             }
             #[pyo3(name = "to_bytes")]
-            pub fn py_to_bytes<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
+            pub fn py_to_bytes<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<pyo3::Bound<'p, pyo3::types::PyBytes>> {
                 let mut writer = Vec::<u8>::new();
                 #crate_name::Streamable::stream(self, &mut writer).map_err(|e| <#crate_name::chia_error::Error as Into<pyo3::PyErr>>::into(e))?;
-                Ok(pyo3::types::PyBytes::new(py, &writer))
+                Ok(pyo3::types::PyBytes::new_bound(py, &writer))
             }
 
-            pub fn stream_to_bytes<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
+            pub fn stream_to_bytes<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<pyo3::Bound<'p, pyo3::types::PyBytes>> {
                 self.py_to_bytes(py)
             }
 
-            pub fn __bytes__<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
+            pub fn __bytes__<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<pyo3::Bound<'p, pyo3::types::PyBytes>> {
                 self.py_to_bytes(py)
             }
 
             pub fn __deepcopy__<'p>(&self, memo: &pyo3::PyAny) -> pyo3::PyResult<Self> {
                 Ok(self.clone())
             }
 
@@ -261,22 +261,22 @@
 
                     Ok(())
                 }
 
                 pub fn __getstate__<'py>(
                     &self,
                     py: pyo3::Python<'py>,
-                ) -> pyo3::PyResult<&'py pyo3::types::PyBytes> {
+                ) -> pyo3::PyResult<pyo3::Bound<'py, pyo3::types::PyBytes>> {
                     self.py_to_bytes(py)
                 }
 
-                pub fn __getnewargs__<'py>(&self, py: pyo3::Python<'py>) -> pyo3::PyResult<&'py pyo3::types::PyTuple> {
+                pub fn __getnewargs__<'py>(&self, py: pyo3::Python<'py>) -> pyo3::PyResult<pyo3::Bound<'py, pyo3::types::PyTuple>> {
                     let mut args = Vec::new();
                     #( args.push(#crate_name::ChiaToPython::to_python(&self.#fnames, py)?); )*
-                    Ok(pyo3::types::PyTuple::new(py, args))
+                    Ok(pyo3::types::PyTuple::new_bound(py, args))
                 }
             }
         };
         py_protocol.extend(pickle);
     }
 
     py_protocol.into()
@@ -312,15 +312,15 @@
                 impl #crate_name::to_json_dict::ToJsonDict for #ident {
                     fn to_json_dict(&self, py: pyo3::Python) -> pyo3::PyResult<pyo3::PyObject> {
                         <u8 as #crate_name::to_json_dict::ToJsonDict>::to_json_dict(&(*self as u8), py)
                     }
                 }
 
                 impl #crate_name::from_json_dict::FromJsonDict for #ident {
-                    fn from_json_dict(o: &pyo3::PyAny) -> pyo3::PyResult<Self> {
+                    fn from_json_dict(o: &pyo3::Bound<pyo3::PyAny>) -> pyo3::PyResult<Self> {
                         let v = <u8 as #crate_name::from_json_dict::FromJsonDict>::from_json_dict(o)?;
                         <Self as #crate_name::Streamable>::parse::<false>(&mut std::io::Cursor::<&[u8]>::new(&[v])).map_err(|e| e.into())
                     }
                 }
             }
             .into();
         }
@@ -342,24 +342,26 @@
 
             let fnames_maybe_upper = maybe_upper_fields(py_uppercase, fnames.clone());
 
             py_protocol.extend( quote! {
 
                 impl #crate_name::to_json_dict::ToJsonDict for #ident {
                     fn to_json_dict(&self, py: pyo3::Python) -> pyo3::PyResult<pyo3::PyObject> {
-                        let ret = pyo3::types::PyDict::new(py);
+                        use pyo3::prelude::PyDictMethods;
+                        let ret = pyo3::types::PyDict::new_bound(py);
                         #(ret.set_item(stringify!(#fnames_maybe_upper), self.#fnames.to_json_dict(py)?)?);*;
                         Ok(ret.into())
                     }
                 }
 
                 impl #crate_name::from_json_dict::FromJsonDict for #ident {
-                    fn from_json_dict(o: &pyo3::PyAny) -> pyo3::PyResult<Self> {
+                    fn from_json_dict(o: &pyo3::Bound<pyo3::PyAny>) -> pyo3::PyResult<Self> {
+                        use pyo3::prelude::PyAnyMethods;
                         Ok(Self{
-                            #(#fnames: <#ftypes as #crate_name::from_json_dict::FromJsonDict>::from_json_dict(o.get_item(stringify!(#fnames_maybe_upper))?)?,)*
+                            #(#fnames: <#ftypes as #crate_name::from_json_dict::FromJsonDict>::from_json_dict(&o.get_item(stringify!(#fnames_maybe_upper))?)?,)*
                         })
                     }
                 }
             });
         }
         _ => {
             panic!("PyJsonDict only supports structs");
@@ -410,15 +412,15 @@
     let fnames_maybe_upper = maybe_upper_fields(py_uppercase, fnames.clone());
 
     let ret = quote! {
         #[pyo3::pymethods]
         impl #ident {
             #(
             #[getter]
-            fn #fnames_maybe_upper<'a> (&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
+            fn #fnames_maybe_upper<'a> (&self, py: pyo3::Python<'a>) -> pyo3::PyResult<pyo3::Bound<'a, pyo3::PyAny>> {
                 #crate_name::ChiaToPython::to_python(&self.#fnames, py)
             }
             )*
         }
     };
 
     ret.into()
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/Cargo.toml` & `chia_rs-0.9.0/crates/chia-bls/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [package]
 name = "chia-bls"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "BLS signature, verification and aggregation funcions for the Chia blockchain"
 authors = ["Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "chia_py_streamable_macro", "chia-traits/py-bindings"]
 arbitrary = ["dep:arbitrary"]
 
 [dependencies]
-chia-traits = { version = "0.8.0", path = "../chia-traits" }
-chia_py_streamable_macro = { version = "0.7.0", path = "../chia_py_streamable_macro", optional = true }
+chia-traits = { version = "0.9.0", path = "../chia-traits" }
+chia_py_streamable_macro = { version = "0.9.0", path = "../chia_py_streamable_macro", optional = true }
 tiny-bip39 = "1.0.0"
 anyhow = "1.0.71"
 sha2 = "0.10.8"
 hkdf = "0.12.0"
 blst = { version = "0.3.11", git = "https://github.com/supranational/blst.git", rev = "0d46eefa45fc1e57aceb42bba0e84eab3a7a9725", features = ["portable"] }
 hex = "0.4.3"
 thiserror = "1.0.44"
-pyo3 = { version = "0.19.0", features = ["multiple-pymethods"], optional = true }
+pyo3 = { version = "0.21.2", features = ["multiple-pymethods"], optional = true }
 arbitrary = { version = "1.3.0" , optional = true}
 lru = "0.12.2"
 
 
 [dev-dependencies]
 rand = "0.8.5"
 criterion = "0.5.1"
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/README.md` & `chia_rs-0.9.0/crates/chia-bls/README.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/benches/cache.rs` & `chia_rs-0.9.0/crates/chia-bls/benches/cache.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 use chia_bls::aggregate_verify;
-use chia_bls::{sign, BLSCache, PublicKey, SecretKey, Signature};
+use chia_bls::{sign, BlsCache, SecretKey, Signature};
 use criterion::{criterion_group, criterion_main, Criterion};
 use rand::rngs::StdRng;
 use rand::{Rng, SeedableRng};
 
 fn cache_benchmark(c: &mut Criterion) {
     let mut rng = StdRng::seed_from_u64(1337);
     let mut data = [0u8; 32];
     rng.fill(data.as_mut_slice());
 
     let sk = SecretKey::from_seed(&data);
     let msg = b"The quick brown fox jumps over the lazy dog";
 
-    let mut pks = Vec::<PublicKey>::new();
+    let mut pks = Vec::new();
 
     let mut agg_sig = Signature::default();
     for i in 0..1000 {
         let derived = sk.derive_hardened(i as u32);
         let pk = derived.public_key();
         let sig = sign(&derived, msg);
         agg_sig.aggregate(&sig);
         pks.push(pk);
     }
 
-    let mut bls_cache: BLSCache = BLSCache::default();
+    let mut bls_cache = BlsCache::default();
 
     c.bench_function("bls_cache.aggregate_verify, 0% cache hits", |b| {
         let mut cache = bls_cache.clone();
         b.iter(|| {
             assert!(cache.aggregate_verify(&pks, [&msg].iter().cycle(), &agg_sig));
         });
     });
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/benches/derive_key.rs` & `chia_rs-0.9.0/crates/chia-bls/benches/derive_key.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/benches/parse.rs` & `chia_rs-0.9.0/crates/chia-bls/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/benches/sign.rs` & `chia_rs-0.9.0/crates/chia-bls/benches/sign.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/benches/verify.rs` & `chia_rs-0.9.0/crates/chia-bls/benches/verify.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/derive_keys.rs` & `chia_rs-0.9.0/crates/chia-bls/src/derive_keys.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/error.rs` & `chia_rs-0.9.0/crates/chia-bls/src/error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/gtelement.rs` & `chia_rs-0.9.0/crates/chia-bls/src/gtelement.rs`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 #[cfg(feature = "py-bindings")]
 use chia_traits::from_json_dict::FromJsonDict;
 #[cfg(feature = "py-bindings")]
 use chia_traits::to_json_dict::ToJsonDict;
 #[cfg(feature = "py-bindings")]
 use pyo3::exceptions::PyValueError;
 #[cfg(feature = "py-bindings")]
+use pyo3::types::PyAnyMethods;
+#[cfg(feature = "py-bindings")]
 use pyo3::{pyclass, pymethods, IntoPy, PyAny, PyObject, PyResult, Python};
 
 #[cfg_attr(feature = "py-bindings", pyclass, derive(PyStreamable))]
 #[derive(Clone)]
 pub struct GTElement(pub(crate) blst_fp12);
 
 impl GTElement {
@@ -112,15 +114,15 @@
         let bytes = self.to_bytes();
         Ok(hex::encode(bytes).into_py(py))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl FromJsonDict for GTElement {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &pyo3::Bound<PyAny>) -> PyResult<Self> {
         let s: String = o.extract()?;
         if !s.starts_with("0x") {
             return Err(PyValueError::new_err(
                 "bytes object is expected to start with 0x",
             ));
         }
         let s = &s[2..];
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/lib.rs` & `chia_rs-0.9.0/crates/chia-bls/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pub mod error;
 pub mod gtelement;
 pub mod mnemonic;
 pub mod public_key;
 pub mod secret_key;
 pub mod signature;
 
-pub use cached_bls::BLSCache;
+pub use cached_bls::BlsCache;
 pub use derivable_key::DerivableKey;
 pub use error::{Error, Result};
 pub use gtelement::GTElement;
 pub use public_key::{hash_to_g1, hash_to_g1_with_dst, PublicKey};
 pub use secret_key::SecretKey;
 pub use signature::{
     aggregate, aggregate_pairing, aggregate_verify, aggregate_verify_gt, hash_to_g2,
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/mnemonic.rs` & `chia_rs-0.9.0/crates/chia-bls/src/mnemonic.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/public_key.rs` & `chia_rs-0.9.0/crates/chia-bls/src/public_key.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 #[cfg(feature = "py-bindings")]
 use chia_py_streamable_macro::PyStreamable;
 #[cfg(feature = "py-bindings")]
 use chia_traits::from_json_dict::FromJsonDict;
 #[cfg(feature = "py-bindings")]
 use chia_traits::to_json_dict::ToJsonDict;
 #[cfg(feature = "py-bindings")]
+use pyo3::prelude::PyAnyMethods;
+#[cfg(feature = "py-bindings")]
 use pyo3::{pyclass, pymethods, IntoPy, PyAny, PyObject, PyResult, Python};
 
 #[cfg_attr(
     feature = "py-bindings",
     pyclass(name = "G1Element"),
     derive(PyStreamable)
 )]
@@ -128,14 +130,18 @@
 
     pub fn is_valid(&self) -> bool {
         // Infinity was considered a valid G1Element in older Relic versions
         // For historical compatibililty this behavior is maintained.
         unsafe { blst_p1_is_inf(&self.0) || blst_p1_in_g1(&self.0) }
     }
 
+    pub fn is_inf(&self) -> bool {
+        unsafe { blst_p1_is_inf(&self.0) }
+    }
+
     pub fn negate(&mut self) {
         unsafe {
             blst_p1_cneg(&mut self.0, true);
         }
     }
 
     pub fn scalar_multiply(&mut self, int_bytes: &[u8]) {
@@ -297,15 +303,15 @@
     fn to_json_dict(&self, py: Python) -> pyo3::PyResult<PyObject> {
         let bytes = self.to_bytes();
         Ok(("0x".to_string() + &hex::encode(bytes)).into_py(py))
     }
 }
 
 #[cfg(feature = "py-bindings")]
-pub fn parse_hex_string(o: &PyAny, len: usize, name: &str) -> PyResult<Vec<u8>> {
+pub fn parse_hex_string(o: &pyo3::Bound<PyAny>, len: usize, name: &str) -> PyResult<Vec<u8>> {
     use pyo3::exceptions::{PyTypeError, PyValueError};
     if let Ok(s) = o.extract::<String>() {
         let s = if let Some(st) = s.strip_prefix("0x") {
             st
         } else {
             &s[..]
         };
@@ -342,15 +348,15 @@
             name
         )))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl FromJsonDict for PublicKey {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &pyo3::Bound<PyAny>) -> PyResult<Self> {
         Ok(Self::from_bytes(
             parse_hex_string(o, 48, "PublicKey")?
                 .as_slice()
                 .try_into()
                 .unwrap(),
         )?)
     }
@@ -545,14 +551,40 @@
             let sk = SecretKey::from_seed(&data);
             let pk = sk.public_key();
             assert!(pk.is_valid());
         }
     }
 
     #[test]
+    fn test_default_is_inf() {
+        let pk = PublicKey::default();
+        assert!(pk.is_inf());
+    }
+
+    #[test]
+    fn test_infinity() {
+        let mut data = [0u8; 48];
+        data[0] = 0xc0;
+        let pk = PublicKey::from_bytes(&data).unwrap();
+        assert!(pk.is_inf());
+    }
+
+    #[test]
+    fn test_is_inf() {
+        let mut rng = StdRng::seed_from_u64(1337);
+        let mut data = [0u8; 32];
+        for _i in 0..500 {
+            rng.fill(data.as_mut_slice());
+            let sk = SecretKey::from_seed(&data);
+            let pk = sk.public_key();
+            assert!(!pk.is_inf());
+        }
+    }
+
+    #[test]
     fn test_hash() {
         fn hash<T: std::hash::Hash>(v: T) -> u64 {
             use std::collections::hash_map::DefaultHasher;
             let mut h = DefaultHasher::new();
             v.hash(&mut h);
             h.finish()
         }
@@ -737,15 +769,15 @@
         let mut data = [0u8; 32];
         for _i in 0..50 {
             rng.fill(data.as_mut_slice());
             let sk = SecretKey::from_seed(&data);
             let pk = sk.public_key();
             Python::with_gil(|py| {
                 let string = pk.to_json_dict(py).expect("to_json_dict");
-                let pk2 = PublicKey::from_json_dict(string.as_ref(py)).unwrap();
+                let pk2 = PublicKey::from_json_dict(string.bind(py)).unwrap();
                 assert_eq!(pk, pk2);
             });
         }
     }
 
     #[rstest]
     #[case("0x000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e", "PublicKey, invalid length 47 expected 48")]
@@ -753,12 +785,12 @@
     #[case("000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e", "PublicKey, invalid length 47 expected 48")]
     #[case("000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f00", "PublicKey, invalid length 49 expected 48")]
     #[case("0x00r102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f", "invalid hex")]
     fn test_json_dict(#[case] input: &str, #[case] msg: &str) {
         pyo3::prepare_freethreaded_python();
         Python::with_gil(|py| {
             let err =
-                PublicKey::from_json_dict(input.to_string().into_py(py).as_ref(py)).unwrap_err();
-            assert_eq!(err.value(py).to_string(), msg.to_string());
+                PublicKey::from_json_dict(input.to_string().into_py(py).bind(py)).unwrap_err();
+            assert_eq!(err.value_bound(py).to_string(), msg.to_string());
         });
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/secret_key.rs` & `chia_rs-0.9.0/crates/chia-bls/src/secret_key.rs`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         let bytes = self.to_bytes();
         Ok(("0x".to_string() + &hex::encode(bytes)).into_py(py))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl FromJsonDict for SecretKey {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &pyo3::Bound<PyAny>) -> PyResult<Self> {
         Ok(Self::from_bytes(
             parse_hex_string(o, 32, "PrivateKey")?
                 .as_slice()
                 .try_into()
                 .unwrap(),
         )?)
     }
@@ -522,15 +522,15 @@
         let mut rng = StdRng::seed_from_u64(1337);
         let mut data = [0u8; 32];
         for _i in 0..50 {
             rng.fill(data.as_mut_slice());
             let sk = SecretKey::from_seed(&data);
             Python::with_gil(|py| {
                 let string = sk.to_json_dict(py).expect("to_json_dict");
-                let sk2 = SecretKey::from_json_dict(string.as_ref(py)).unwrap();
+                let sk2 = SecretKey::from_json_dict(string.bind(py)).unwrap();
                 assert_eq!(sk, sk2);
                 assert_eq!(sk.public_key(), sk2.public_key());
             });
         }
     }
 
     #[rstest]
@@ -554,12 +554,12 @@
         "0r0102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f",
         "invalid hex"
     )]
     fn test_json_dict(#[case] input: &str, #[case] msg: &str) {
         pyo3::prepare_freethreaded_python();
         Python::with_gil(|py| {
             let err =
-                SecretKey::from_json_dict(input.to_string().into_py(py).as_ref(py)).unwrap_err();
-            assert_eq!(err.value(py).to_string(), msg.to_string());
+                SecretKey::from_json_dict(input.to_string().into_py(py).bind(py)).unwrap_err();
+            assert_eq!(err.value_bound(py).to_string(), msg.to_string());
         });
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-bls/src/signature.rs` & `chia_rs-0.9.0/crates/chia-bls/src/signature.rs`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         let bytes = self.to_bytes();
         Ok(("0x".to_string() + &hex::encode(bytes)).into_py(py))
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl FromJsonDict for Signature {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &pyo3::Bound<PyAny>) -> PyResult<Self> {
         Ok(Self::from_bytes(
             parse_hex_string(o, 96, "Signature")?
                 .as_slice()
                 .try_into()
                 .unwrap(),
         )?)
     }
@@ -1254,15 +1254,15 @@
         for _i in 0..50 {
             rng.fill(data.as_mut_slice());
             rng.fill(msg.as_mut_slice());
             let sk = SecretKey::from_seed(&data);
             let sig = sign(&sk, msg);
             Python::with_gil(|py| {
                 let string = sig.to_json_dict(py).expect("to_json_dict");
-                let sig2 = Signature::from_json_dict(string.as_ref(py)).unwrap();
+                let sig2 = Signature::from_json_dict(string.bind(py)).unwrap();
                 assert_eq!(sig, sig2);
             });
         }
     }
 
     #[rstest]
     #[case("0x000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0ff000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e", "Signature, invalid length 95 expected 96")]
@@ -1270,12 +1270,12 @@
     #[case("000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0ff000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e", "Signature, invalid length 95 expected 96")]
     #[case("000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0ff000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f00", "Signature, invalid length 97 expected 96")]
     #[case("00r102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0ff000102030405060708090a0b0c0d0e0f000102030405060708090a0b0c0d0e0f", "invalid hex")]
     fn test_json_dict(#[case] input: &str, #[case] msg: &str) {
         pyo3::prepare_freethreaded_python();
         Python::with_gil(|py| {
             let err =
-                Signature::from_json_dict(input.to_string().into_py(py).as_ref(py)).unwrap_err();
-            assert_eq!(err.value(py).to_string(), msg.to_string());
+                Signature::from_json_dict(input.to_string().into_py(py).bind(py)).unwrap_err();
+            assert_eq!(err.value_bound(py).to_string(), msg.to_string());
         });
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia_streamable_macro/Cargo.toml` & `chia_rs-0.9.0/crates/chia_streamable_macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia_streamable_macro/src/lib.rs` & `chia_rs-0.9.0/crates/chia_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-utils/Cargo.toml` & `chia_rs-0.9.0/crates/clvm-utils/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "clvm-utils"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions for processing clvm programs and structures"
 authors = ["Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 
 [dependencies]
 clvmr = "0.7.0"
-clvm-traits = { version = "0.8.0", path = "../clvm-traits" }
+clvm-traits = { version = "0.9.0", path = "../clvm-traits" }
 hex = "0.4.3"
 
 [dev-dependencies]
 rstest = "0.16.0"
-clvm-traits = { version = "0.8.0", path = "../clvm-traits", features = ["derive"] }
+clvm-traits = { version = "0.9.0", path = "../clvm-traits", features = ["derive"] }
```

### Comparing `chia_rs-0.8.0/crates/clvm-utils/src/curried_program.rs` & `chia_rs-0.9.0/crates/clvm-utils/src/curried_program.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-utils/src/curry_tree_hash.rs` & `chia_rs-0.9.0/crates/clvm-utils/src/curry_tree_hash.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-utils/src/hash_encoder.rs` & `chia_rs-0.9.0/crates/clvm-utils/src/hash_encoder.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-utils/src/lib.rs` & `chia_rs-0.9.0/crates/clvm-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-utils/src/tree_hash.rs` & `chia_rs-0.9.0/crates/clvm-utils/src/tree_hash.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-derive/src/from_clvm.rs` & `chia_rs-0.9.0/crates/clvm-derive/src/to_clvm.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,334 +1,311 @@
-use proc_macro2::{Ident, Literal, Span, TokenStream};
-use quote::quote;
-use syn::{
-    parse_quote, spanned::Spanned, Data, DeriveInput, Expr, Fields, FieldsNamed, FieldsUnnamed,
-    GenericParam, Type,
-};
+use proc_macro2::{Span, TokenStream};
+use quote::{quote, ToTokens};
+use syn::{parse_quote, DeriveInput, GenericParam, Ident, Index};
 
 use crate::{
-    helpers::{add_trait_bounds, parse_clvm_attr, parse_int_repr, Repr},
-    macros::{repr_macros, Macros},
+    crate_name,
+    helpers::{add_trait_bounds, variant_discriminants, DiscriminantInfo},
+    parser::{parse, EnumInfo, FieldInfo, ParsedInfo, Repr, StructInfo, StructKind, VariantKind},
 };
 
-#[derive(Default)]
-struct FieldInfo {
-    field_types: Vec<Type>,
-    field_names: Vec<Ident>,
-    initializer: TokenStream,
-}
+pub fn to_clvm(ast: DeriveInput) -> TokenStream {
+    let parsed = parse("ToClvm", &ast);
+    let node_name = Ident::new("Node", Span::mixed_site());
 
-struct VariantInfo {
-    name: Ident,
-    discriminant: Expr,
-    field_info: FieldInfo,
-    macros: Macros,
+    match parsed {
+        ParsedInfo::Struct(struct_info) => impl_for_struct(ast, struct_info, node_name),
+        ParsedInfo::Enum(enum_info) => impl_for_enum(ast, enum_info, node_name),
+    }
 }
 
-pub fn from_clvm(ast: DeriveInput) -> TokenStream {
-    let clvm_attr = parse_clvm_attr(&ast.attrs);
-    let crate_name = quote!(clvm_traits);
-
-    match &ast.data {
-        Data::Struct(data_struct) => {
-            if clvm_attr.untagged {
-                panic!("cannot use `untagged` on a struct");
-            }
-            let macros = repr_macros(&crate_name, clvm_attr.expect_repr());
-            let field_info = fields(&data_struct.fields);
-            impl_for_struct(&crate_name, &ast, &macros, &field_info)
-        }
-        Data::Enum(data_enum) => {
-            if !clvm_attr.untagged && clvm_attr.repr == Some(Repr::Curry) {
-                panic!("cannot use `curry` on a tagged enum, since unlike other representations, each argument is wrapped");
-            }
+fn encode_fields(
+    crate_name: &Ident,
+    node_name: &Ident,
+    fields: &[FieldInfo],
+    repr: Repr,
+) -> TokenStream {
+    let mut body = TokenStream::new();
+    let mut value_names = Vec::new();
 
-            let mut next_discriminant: Expr = parse_quote!(0);
-            let mut variants = Vec::new();
+    // Generate the values that need to be encoded for each field.
+    // As well as a unique name for each field to reference later.
+    for (i, field) in fields.iter().enumerate() {
+        let value_name = Ident::new(&format!("field_{}", i), Span::mixed_site());
+
+        if let Some(value) = &field.constant {
+            body.extend(quote! {
+                // Use the constant's value directly, since it's not in `self`.
+                let #value_name = #value;
+            });
+        }
 
-            for variant in data_enum.variants.iter() {
-                let field_info = fields(&variant.fields);
-                let variant_clvm_attr = parse_clvm_attr(&variant.attrs);
+        value_names.push(value_name);
+    }
 
-                if variant_clvm_attr.untagged {
-                    panic!("cannot use `untagged` on an enum variant");
-                }
+    let encode_next = match repr {
+        Repr::Atom | Repr::Transparent => unreachable!(),
+        // Encode `(A . B)` pairs for lists.
+        Repr::List => quote!(encode_pair),
+        // Encode `(c (q . A) B)` pairs for curried arguments.
+        Repr::Curry => quote!(encode_curried_arg),
+    };
 
-                let repr = variant_clvm_attr
-                    .repr
-                    .unwrap_or_else(|| clvm_attr.expect_repr());
-                if !clvm_attr.untagged && repr == Repr::Curry {
-                    panic!("cannot use `curry` on a tagged enum variant, since unlike other representations, each argument is wrapped");
-                }
+    let initial_value = match repr {
+        Repr::Atom | Repr::Transparent => unreachable!(),
+        Repr::List => quote!(encoder.encode_atom(&[])?),
+        Repr::Curry => quote!(encoder.encode_atom(&[1])?),
+    };
 
-                let macros = repr_macros(&crate_name, repr);
-                let variant_info = VariantInfo {
-                    name: variant.ident.clone(),
-                    discriminant: variant
-                        .discriminant
-                        .as_ref()
-                        .map(|(_, discriminant)| {
-                            next_discriminant = parse_quote!(#discriminant + 1);
-                            discriminant.clone()
-                        })
-                        .unwrap_or_else(|| {
-                            let discriminant = next_discriminant.clone();
-                            next_discriminant = parse_quote!(#next_discriminant + 1);
-                            discriminant
-                        }),
-                    field_info,
-                    macros,
-                };
-                variants.push(variant_info);
-            }
+    // We're going to build the return value in reverse order, so we need to start with the terminator.
+    body.extend(quote! {
+        let mut node = #initial_value;
+    });
+
+    for (i, field) in fields.iter().enumerate().rev() {
+        let value_name = &value_names[i];
+        let ty = &field.ty;
+
+        let mut if_body = TokenStream::new();
+
+        // Encode the field value.
+        if_body.extend(quote! {
+            let value_node = <#ty as #crate_name::ToClvm<#node_name>>::to_clvm(&#value_name, encoder)?;
+        });
+
+        if field.rest {
+            // This field represents the rest of the arguments, so we can replace the terminator with it.
+            if_body.extend(quote! {
+                node = value_node;
+            });
+        } else {
+            // Prepend the field value to the existing node with a new pair.
+            if_body.extend(quote! {
+                node = encoder.#encode_next(value_node, node)?;
+            });
+        }
 
-            if clvm_attr.untagged {
-                impl_for_untagged_enum(&crate_name, &ast, &variants)
-            } else {
-                let int_repr = parse_int_repr(&ast.attrs);
-                impl_for_enum(&crate_name, &ast, &int_repr, &variants)
-            }
+        if let Some(default) = &field.optional_with_default {
+            let default = default
+                .as_ref()
+                .map(|expr| expr.to_token_stream())
+                .unwrap_or_else(|| quote!(<#ty as ::std::default::Default>::default()));
+
+            // If the field is equal to the default value, don't encode it.
+            body.extend(quote! {
+                if #value_name != &#default {
+                    #if_body
+                }
+            });
+        } else {
+            // Encode the field unconditionally if it's not optional.
+            body.extend(if_body);
         }
-        Data::Union(_union) => panic!("cannot derive `FromClvm` for a union"),
     }
-}
 
-fn fields(fields: &Fields) -> FieldInfo {
-    match fields {
-        Fields::Named(fields) => named_fields(fields),
-        Fields::Unnamed(fields) => unnamed_fields(fields),
-        Fields::Unit => FieldInfo::default(),
-    }
+    body
 }
 
-fn named_fields(fields: &FieldsNamed) -> FieldInfo {
-    let fields = &fields.named;
-    let field_types = fields.iter().map(|field| field.ty.clone()).collect();
-    let field_names: Vec<Ident> = fields
-        .iter()
-        .map(|field| field.ident.clone().unwrap())
-        .collect();
-    let initializer = quote!({ #( #field_names, )* });
-
-    FieldInfo {
-        field_types,
-        field_names,
-        initializer,
-    }
-}
+fn impl_for_struct(ast: DeriveInput, struct_info: StructInfo, node_name: Ident) -> TokenStream {
+    let crate_name = crate_name(struct_info.crate_name);
 
-fn unnamed_fields(fields: &FieldsUnnamed) -> FieldInfo {
-    let fields = &fields.unnamed;
-    let field_types = fields.iter().map(|field| field.ty.clone()).collect();
-    let field_names: Vec<Ident> = fields
-        .iter()
-        .enumerate()
-        .map(|(i, field)| Ident::new(&format!("field_{i}"), field.span()))
-        .collect();
-    let initializer = quote!(( #( #field_names, )* ));
-
-    FieldInfo {
-        field_types,
-        field_names,
-        initializer,
-    }
-}
+    let mut body = TokenStream::new();
 
-fn impl_for_struct(
-    crate_name: &TokenStream,
-    ast: &DeriveInput,
-    Macros {
-        match_macro,
-        destructure_macro,
-        ..
-    }: &Macros,
-    FieldInfo {
-        field_types,
-        field_names,
-        initializer,
-    }: &FieldInfo,
-) -> TokenStream {
-    let node_name = Ident::new("Node", Span::mixed_site());
+    for (i, field) in struct_info.fields.iter().enumerate() {
+        // We can't encode fields that are constant, since they aren't on the actual struct.
+        if field.constant.is_some() {
+            continue;
+        }
 
-    let body = quote! {
-        let #destructure_macro!( #( #field_names, )* ) =
-            <#match_macro!( #( #field_types ),* )
-            as #crate_name::FromClvm<#node_name>>::from_clvm(decoder, node)?;
-        Ok(Self #initializer)
-    };
+        // Rename the field so it doesn't clash with anything else in scope such as `node`.
+        let value_name = Ident::new(&format!("field_{}", i), Span::mixed_site());
+
+        match struct_info.kind {
+            StructKind::Named => {
+                let field_name = &field.ident;
+                body.extend(quote! {
+                    let #value_name = &self.#field_name;
+                });
+            }
+            StructKind::Unnamed => {
+                let field_index = Index::from(i);
+                body.extend(quote! {
+                    let #value_name = &self.#field_index;
+                });
+            }
+            StructKind::Unit => unreachable!(),
+        }
+    }
+
+    body.extend(encode_fields(
+        &crate_name,
+        &node_name,
+        &struct_info.fields,
+        struct_info.repr,
+    ));
+
+    body.extend(quote! {
+        Ok(node)
+    });
 
-    generate_from_clvm(crate_name, ast, &node_name, &body)
+    trait_impl(ast, crate_name, node_name, body)
 }
 
-fn impl_for_enum(
-    crate_name: &TokenStream,
-    ast: &DeriveInput,
-    int_repr: &Ident,
-    variants: &[VariantInfo],
-) -> TokenStream {
-    let type_name = Literal::string(&ast.ident.to_string());
-    let node_name = Ident::new("Node", Span::mixed_site());
+fn impl_for_enum(ast: DeriveInput, enum_info: EnumInfo, node_name: Ident) -> TokenStream {
+    let crate_name = crate_name(enum_info.crate_name.clone());
 
-    let mut discriminant_definitions = Vec::new();
-    let mut has_initializers = false;
+    let mut variant_destructures = Vec::new();
 
-    let variant_bodies = variants
-        .iter()
-        .enumerate()
-        .map(|(i, variant_info)| {
-            let VariantInfo {
-                name,
-                discriminant,
-                field_info,
-                macros,
-            } = variant_info;
-
-            let FieldInfo {
-                field_types,
-                field_names,
-                initializer,
-            } = field_info;
-
-            let Macros {
-                match_macro,
-                destructure_macro,
-                ..
-            } = macros;
-
-            let discriminant_ident = Ident::new(&format!("VALUE_{}", i), Span::mixed_site());
-            discriminant_definitions.push(quote! {
-                const #discriminant_ident: #int_repr = #discriminant;
-            });
+    for variant in enum_info.variants.iter() {
+        let variant_name = &variant.name;
 
-            if initializer.is_empty() {
-                quote! {
-                    #discriminant_ident => {
-                        Ok(Self::#name)
-                    }
-                }
-            } else {
-                has_initializers = true;
-                quote! {
-                    #discriminant_ident => {
-                        let #destructure_macro!( #( #field_names ),* ) =
-                            <#match_macro!( #( #field_types ),* )
-                            as #crate_name::FromClvm<#node_name>>::from_clvm(decoder, args.0)?;
-                        Ok(Self::#name #initializer)
-                    }
-                }
+        let field_names: Vec<Ident> = variant
+            .fields
+            .iter()
+            .map(|field| field.ident.clone())
+            .collect();
+
+        let value_names: Vec<Ident> = (0..variant.fields.len())
+            .map(|i| Ident::new(&format!("field_{}", i), Span::mixed_site()))
+            .collect();
+
+        let destructure = match variant.kind {
+            VariantKind::Unit => quote!(Self::#variant_name),
+            VariantKind::Unnamed => {
+                quote!(Self::#variant_name( #( #value_names, )* ))
+            }
+            VariantKind::Named => {
+                quote!(Self::#variant_name { #( #field_names: #value_names, )* })
             }
-        })
-        .collect::<Vec<_>>();
+        };
 
-    let parse_value = if has_initializers {
-        quote! {
-            let (value, args) = <(#int_repr, #crate_name::Raw<#node_name>)>::from_clvm(decoder, node)?;
-        }
-    } else {
-        quote! {
-            let value = #int_repr::from_clvm(decoder, node)?;
-        }
-    };
+        variant_destructures.push(destructure);
+    }
 
-    let body = quote! {
-        #parse_value
+    let body = if enum_info.is_untagged {
+        let mut variant_bodies = Vec::new();
 
-        #( #discriminant_definitions )*
+        for variant in enum_info.variants.iter() {
+            let repr = variant.repr.unwrap_or(enum_info.default_repr);
 
-        match value {
-            #( #variant_bodies )*
-            _ => Err(#crate_name::FromClvmError::Custom(
-                format!("failed to match any enum variants of `{}`", #type_name)
-            ))
+            variant_bodies.push(encode_fields(
+                &crate_name,
+                &node_name,
+                &variant.fields,
+                repr,
+            ));
         }
-    };
-
-    generate_from_clvm(crate_name, ast, &node_name, &body)
-}
 
-fn impl_for_untagged_enum(
-    crate_name: &TokenStream,
-    ast: &DeriveInput,
-    variants: &[VariantInfo],
-) -> TokenStream {
-    let type_name = Literal::string(&ast.ident.to_string());
-    let node_name = Ident::new("Node", Span::mixed_site());
-
-    let variant_bodies = variants
-        .iter()
-        .map(|variant_info| {
-            let VariantInfo {
-                name,
-                field_info,
-                macros,
-                ..
-            } = variant_info;
-
-            let FieldInfo {
-                field_types,
-                field_names,
-                initializer,
-            } = field_info;
-
-            let Macros {
-                match_macro,
-                destructure_macro,
-                ..
-            } = macros;
+        // Encode the variant's fields directly.
+        quote! {
+            match self {
+                #( #variant_destructures => {
+                    #variant_bodies
+                    Ok(node)
+                }, )*
+            }
+        }
+    } else {
+        let DiscriminantInfo {
+            discriminant_type,
+            discriminant_consts,
+            discriminant_names,
+            variant_names,
+        } = variant_discriminants(&enum_info);
 
+        if enum_info.default_repr == Repr::Atom {
+            // Encode the discriminant by itself as an atom.
             quote! {
-                if let Ok(#destructure_macro!( #( #field_names ),* )) =
-                    <#match_macro!( #( #field_types ),* )
-                    as #crate_name::FromClvm<#node_name>>::from_clvm(decoder, decoder.clone_node(&node))
-                {
-                    return Ok(Self::#name #initializer);
+                #( #discriminant_consts )*
+
+                match self {
+                    #( Self::#variant_names => {
+                        <#discriminant_type as #crate_name::ToClvm<#node_name>>::to_clvm(
+                            &#discriminant_names,
+                            encoder,
+                        )
+                    }, )*
                 }
             }
-        })
-        .collect::<Vec<_>>();
+        } else {
+            let encode_next = match enum_info.default_repr {
+                Repr::Atom | Repr::Transparent => unreachable!(),
+                // Encode `(A . B)` pairs for lists.
+                Repr::List => quote!(encode_pair),
+                // Encode `(c (q . A) B)` pairs for curried arguments.
+                Repr::Curry => quote!(encode_curried_arg),
+            };
+
+            let mut variant_bodies = Vec::new();
+
+            for variant in enum_info.variants.iter() {
+                let repr = variant.repr.unwrap_or(enum_info.default_repr);
+                variant_bodies.push(encode_fields(
+                    &crate_name,
+                    &node_name,
+                    &variant.fields,
+                    repr,
+                ));
+            }
+
+            // Encode the discriminant followed by the variant's fields.
+            quote! {
+                #( #discriminant_consts )*
 
-    let body = quote! {
-        #( #variant_bodies )*
+                match self {
+                    #( #variant_destructures => {
+                        #variant_bodies
+
+                        let discriminant_node = <#discriminant_type as #crate_name::ToClvm<#node_name>>::to_clvm(
+                            &#discriminant_names,
+                            encoder,
+                        )?;
 
-        Err(#crate_name::FromClvmError::Custom(
-            format!("failed to match any enum variants of `{}`", #type_name)
-        ))
+                        encoder.#encode_next( discriminant_node, node )
+                    }, )*
+                }
+            }
+        }
     };
 
-    generate_from_clvm(crate_name, ast, &node_name, &body)
+    trait_impl(ast, crate_name, node_name, body)
 }
 
-fn generate_from_clvm(
-    crate_name: &TokenStream,
-    ast: &DeriveInput,
-    node_name: &Ident,
-    body: &TokenStream,
+fn trait_impl(
+    mut ast: DeriveInput,
+    crate_name: Ident,
+    node_name: Ident,
+    body: TokenStream,
 ) -> TokenStream {
-    let mut ast = ast.clone();
     let type_name = ast.ident;
 
+    // Every generic type must implement `ToClvm` as well in order for the derived type to implement `ToClvm`.
+    // This isn't always perfect, but it's how derive macros work.
     add_trait_bounds(
         &mut ast.generics,
-        parse_quote!(#crate_name::FromClvm<#node_name>),
+        parse_quote!(#crate_name::ToClvm<#node_name>),
     );
 
     let generics_clone = ast.generics.clone();
+
     let (_, ty_generics, where_clause) = generics_clone.split_for_impl();
 
     ast.generics
         .params
         .push(GenericParam::Type(node_name.clone().into()));
+
     let (impl_generics, _, _) = ast.generics.split_for_impl();
 
+    // Generate the final trait implementation.
     quote! {
         #[automatically_derived]
-        impl #impl_generics #crate_name::FromClvm<#node_name>
+        impl #impl_generics #crate_name::ToClvm<#node_name>
         for #type_name #ty_generics #where_clause {
-            fn from_clvm(
-                decoder: &impl #crate_name::ClvmDecoder<Node = #node_name>,
-                node: #node_name,
-            ) -> ::std::result::Result<Self, #crate_name::FromClvmError> {
+            fn to_clvm(
+                &self,
+                encoder: &mut impl #crate_name::ClvmEncoder<Node = #node_name>
+            ) -> ::std::result::Result<#node_name, #crate_name::ToClvmError> {
                 #body
             }
         }
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-traits/src/chia_error.rs` & `chia_rs-0.9.0/crates/chia-traits/src/chia_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-traits/src/from_json_dict.rs` & `chia_rs-0.9.0/crates/chia-traits/src/from_json_dict.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 use pyo3::exceptions::PyValueError;
+use pyo3::types::PyAnyMethods;
+use pyo3::Bound;
 use pyo3::PyAny;
 use pyo3::PyResult;
 
 pub trait FromJsonDict {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self>
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self>
     where
         Self: Sized;
 }
 
 impl<T> FromJsonDict for Option<T>
 where
     T: FromJsonDict,
 {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         if o.is_none() {
             return Ok(None);
         }
         Ok(Some(<T as FromJsonDict>::from_json_dict(o)?))
     }
 }
 
 macro_rules! from_json_primitive {
     ($t:ty) => {
         impl $crate::from_json_dict::FromJsonDict for $t {
-            fn from_json_dict(o: &pyo3::PyAny) -> pyo3::PyResult<Self> {
+            fn from_json_dict(o: &Bound<PyAny>) -> pyo3::PyResult<Self> {
                 o.extract()
             }
         }
     };
 }
 
 from_json_primitive!(bool);
@@ -43,55 +45,55 @@
 from_json_primitive!(i128);
 from_json_primitive!(String);
 
 impl<T> FromJsonDict for Vec<T>
 where
     T: FromJsonDict,
 {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         let mut ret = Vec::<T>::new();
         for v in o.iter()? {
-            ret.push(<T as FromJsonDict>::from_json_dict(v?)?);
+            ret.push(<T as FromJsonDict>::from_json_dict(&v?)?);
         }
         Ok(ret)
     }
 }
 
 impl<T, U> FromJsonDict for (T, U)
 where
     T: FromJsonDict,
     U: FromJsonDict,
 {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         if o.len()? != 2 {
             return Err(PyValueError::new_err(format!(
                 "expected 2 elements, got {}",
                 o.len()?
             )));
         }
         Ok((
-            <T as FromJsonDict>::from_json_dict(o.get_item(0)?)?,
-            <U as FromJsonDict>::from_json_dict(o.get_item(1)?)?,
+            <T as FromJsonDict>::from_json_dict(&o.get_item(0)?)?,
+            <U as FromJsonDict>::from_json_dict(&o.get_item(1)?)?,
         ))
     }
 }
 
 impl<T, U, V> FromJsonDict for (T, U, V)
 where
     T: FromJsonDict,
     U: FromJsonDict,
     V: FromJsonDict,
 {
-    fn from_json_dict(o: &PyAny) -> PyResult<Self> {
+    fn from_json_dict(o: &Bound<PyAny>) -> PyResult<Self> {
         if o.len()? != 3 {
             return Err(PyValueError::new_err(format!(
                 "expected 3 elements, got {}",
                 o.len()?
             )));
         }
         Ok((
-            <T as FromJsonDict>::from_json_dict(o.get_item(0)?)?,
-            <U as FromJsonDict>::from_json_dict(o.get_item(1)?)?,
-            <V as FromJsonDict>::from_json_dict(o.get_item(2)?)?,
+            <T as FromJsonDict>::from_json_dict(&o.get_item(0)?)?,
+            <U as FromJsonDict>::from_json_dict(&o.get_item(1)?)?,
+            <V as FromJsonDict>::from_json_dict(&o.get_item(2)?)?,
         ))
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-traits/src/int.rs` & `chia_rs-0.9.0/crates/chia-traits/src/int.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-use pyo3::types::{PyAny, PyBool, PyList, PyModule, PyString, PyTuple};
-use pyo3::{IntoPy, PyResult, Python};
+use pyo3::{prelude::*, types::*};
 
 /// A custom to-python conversion trait that turns primitive integer types into
 /// the chia-blockchain fixed-width integer types (uint8, int8, etc.)
 pub trait ChiaToPython {
-    fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::types::PyAny>;
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>>;
 }
 
 macro_rules! primitive_int {
     ($t:ty, $name:expr) => {
         impl ChiaToPython for $t {
-            fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-                let int_module = PyModule::import(py, "chia_rs.sized_ints")?;
+            fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+                let int_module = PyModule::import_bound(py, "chia_rs.sized_ints")?;
                 let ty = int_module.getattr($name)?;
                 ty.call1((self.into_py(py),))
             }
         }
     };
 }
 
@@ -27,58 +26,56 @@
 primitive_int!(u32, "uint32");
 primitive_int!(i64, "int64");
 primitive_int!(u64, "uint64");
 primitive_int!(i128, "int128");
 primitive_int!(u128, "uint128");
 
 impl<T: ChiaToPython> ChiaToPython for Option<T> {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         match &self {
             Some(v) => v.to_python(py),
-            None => Ok(py.None().into_ref(py)),
+            None => Ok(py.None().into_bound(py)),
         }
     }
 }
 
 impl<T: ChiaToPython> ChiaToPython for Vec<T> {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        let ret = PyList::empty(py);
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+        let ret = PyList::empty_bound(py);
         for v in self {
             ret.append(v.to_python(py)?)?;
         }
-        Ok(ret)
+        Ok(ret.into_any())
     }
 }
 
 impl ChiaToPython for bool {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        Ok(PyBool::new(py, *self))
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(PyBool::new_bound(py, *self).as_any().clone())
     }
 }
 
 impl ChiaToPython for String {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        Ok(PyString::new(py, self.as_str()))
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(PyString::new_bound(py, self.as_str()).into_any())
     }
 }
 
 impl<T: ChiaToPython, U: ChiaToPython> ChiaToPython for (T, U) {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        Ok(PyTuple::new(
-            py,
-            [self.0.to_python(py)?, self.1.to_python(py)?],
-        ))
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(PyTuple::new_bound(py, [self.0.to_python(py)?, self.1.to_python(py)?]).into_any())
     }
 }
 
 impl<T: ChiaToPython, U: ChiaToPython, V: ChiaToPython> ChiaToPython for (T, U, V) {
-    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-        Ok(PyTuple::new(
+    fn to_python<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(PyTuple::new_bound(
             py,
             [
                 self.0.to_python(py)?,
                 self.1.to_python(py)?,
                 self.2.to_python(py)?,
             ],
-        ))
+        )
+        .into_any())
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-traits/src/streamable.rs` & `chia_rs-0.9.0/crates/chia-traits/src/streamable.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-traits/src/to_json_dict.rs` & `chia_rs-0.9.0/crates/chia-traits/src/to_json_dict.rs`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 to_json_primitive!(i64);
 to_json_primitive!(u128);
 to_json_primitive!(i128);
 to_json_primitive!(String);
 
 impl<T: ToJsonDict> ToJsonDict for Vec<T> {
     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
-        let list = PyList::empty(py);
+        let list = PyList::empty_bound(py);
         for v in self {
             list.append(v.to_json_dict(py)?)?;
         }
         Ok(list.into())
     }
 }
 
@@ -46,23 +46,23 @@
         }
     }
 }
 
 // if we need more of these, we should probably make a macro
 impl<T: ToJsonDict, U: ToJsonDict> ToJsonDict for (T, U) {
     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
-        let list = PyList::empty(py);
+        let list = PyList::empty_bound(py);
         list.append(self.0.to_json_dict(py)?)?;
         list.append(self.1.to_json_dict(py)?)?;
         Ok(list.into())
     }
 }
 
 impl<T: ToJsonDict, U: ToJsonDict, W: ToJsonDict> ToJsonDict for (T, U, W) {
     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
-        let list = PyList::empty(py);
+        let list = PyList::empty_bound(py);
         list.append(self.0.to_json_dict(py)?)?;
         list.append(self.1.to_json_dict(py)?)?;
         list.append(self.2.to_json_dict(py)?)?;
         Ok(list.into())
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/Cargo.toml` & `chia_rs-0.9.0/crates/chia-consensus/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [package]
 name = "chia-consensus"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions and types used by the Chia blockchain full node"
 authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chia_py_streamable_macro"]
 
 [dependencies]
 clvmr = "0.7.0"
 hex = "0.4.3"
-pyo3 = { version = ">=0.19.0", optional = true }
+pyo3 = { version = "0.21.2", optional = true }
 sha2 = "0.10.8"
 chia_streamable_macro = { version = "0.8.0", path = "../chia_streamable_macro" }
-chia_py_streamable_macro = { version = "0.7.0", path = "../chia_py_streamable_macro", optional = true }
-clvm-utils = { version = "0.8.0", path = "../clvm-utils" }
-chia-traits = { version = "0.8.0", path = "../chia-traits" }
-clvm-traits = { version = "0.8.0", path = "../clvm-traits" }
-clvm-derive = { version = "0.6.0", path = "../clvm-derive" }
-chia-protocol = { version = "0.8.0", path = "../chia-protocol" }
-chia-puzzles = { version = "0.8.0", path = "../chia-puzzles" }
-chia-bls = { version = "0.8.0", path = "../chia-bls" }
+chia_py_streamable_macro = { version = "0.9.0", path = "../chia_py_streamable_macro", optional = true }
+clvm-utils = { version = "0.9.0", path = "../clvm-utils" }
+chia-traits = { version = "0.9.0", path = "../chia-traits" }
+clvm-traits = { version = "0.9.0", path = "../clvm-traits" }
+clvm-derive = { version = "0.9.0", path = "../clvm-derive" }
+chia-protocol = { version = "0.9.0", path = "../chia-protocol" }
+chia-puzzles = { version = "0.9.0", path = "../chia-puzzles" }
+chia-bls = { version = "0.9.0", path = "../chia-bls" }
 hex-literal = "0.4.1"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 num-traits = "0.2.15"
 rstest = "0.16.0"
 text-diff = "0.4.0"
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/README.md` & `chia_rs-0.9.0/crates/chia-consensus/README.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/benches/merkle-set.rs` & `chia_rs-0.9.0/crates/chia-consensus/benches/merkle-set.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/benches/run-generator.rs` & `chia_rs-0.9.0/crates/chia-consensus/benches/run-generator.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/benches/tree-hash.rs` & `chia_rs-0.9.0/crates/chia-consensus/benches/tree-hash.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/consensus_constants.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/consensus_constants.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use chia_protocol::Bytes32;
 use chia_streamable_macro::streamable;
 
 #[cfg(feature = "py-bindings")]
 use chia_py_streamable_macro::{PyGetters, PyJsonDict, PyStreamable};
+use hex_literal::hex;
 
 #[cfg_attr(
     feature = "py-bindings",
     pyo3::pyclass(module = "chia_rs"),
     derive(PyJsonDict, PyStreamable, PyGetters),
     py_uppercase,
     py_pickle
@@ -113,14 +114,17 @@
 
     /// Soft fork initiated in 1.8.0 release.
     soft_fork2_height: u32,
 
     /// Soft fork initiated in 2.3.0 release.
     soft_fork4_height: u32,
 
+    /// Soft fork initiated in 2.4.0 release.
+    soft_fork5_height: u32,
+
     /// The hard fork planned with the 2.0 release.
     /// This is the block with the first plot filter adjustment.
     hard_fork_height: u32,
 
     hard_fork_fix_height: u32,
 
     /// The 128 plot filter adjustment height.
@@ -128,7 +132,61 @@
 
     /// The 64 plot filter adjustment height.
     plot_filter_64_height: u32,
 
     /// The 32 plot filter adjustment height.
     plot_filter_32_height: u32,
 }
+
+pub const TEST_CONSTANTS: ConsensusConstants = ConsensusConstants {
+    slot_blocks_target: 32,
+    min_blocks_per_challenge_block: 16,
+    max_sub_slot_blocks: 128,
+    num_sps_sub_slot: 64,
+    sub_slot_iters_starting: u64::pow(2, 27),
+    difficulty_constant_factor: u128::pow(2, 67),
+    difficulty_starting: 7,
+    difficulty_change_max_factor: 3,
+    sub_epoch_blocks: 384,
+    epoch_blocks: 4608,
+    significant_bits: 8,
+    discriminant_size_bits: 1024,
+    number_zero_bits_plot_filter: 9,
+    min_plot_size: 32,
+    max_plot_size: 50,
+    sub_slot_time_target: 600,
+    num_sp_intervals_extra: 3,
+    max_future_time2: 2 * 60,
+    number_of_timestamps: 11,
+    genesis_challenge: Bytes32::new(hex!(
+        "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
+    )),
+    agg_sig_me_additional_data: Bytes32::new(hex!(
+        "ccd5bb71183532bff220ba46c268991a3ff07eb358e8255a65c30a2dce0e5fbb"
+    )),
+    genesis_pre_farm_pool_puzzle_hash: Bytes32::new(hex!(
+        "d23da14695a188ae5708dd152263c4db883eb27edeb936178d4d988b8f3ce5fc"
+    )),
+    genesis_pre_farm_farmer_puzzle_hash: Bytes32::new(hex!(
+        "3d8765d3a597ec1d99663f6c9816d915b9f68613ac94009884c4addaefcce6af"
+    )),
+    max_vdf_witness_size: 64,
+    mempool_block_buffer: 10,
+    max_coin_amount: u64::MAX,
+    max_block_cost_clvm: 11000000000,
+    cost_per_byte: 12000,
+    weight_proof_threshold: 2,
+    blocks_cache_size: 4608 + (128 * 4),
+    weight_proof_recent_blocks: 1000,
+    max_block_count_per_requests: 32,
+    max_generator_size: 1000000,
+    max_generator_ref_list_size: 512,
+    pool_sub_slot_iters: 37600000000,
+    soft_fork2_height: 0,
+    soft_fork4_height: 5716000,
+    soft_fork5_height: 5940000,
+    hard_fork_height: 5496000,
+    hard_fork_fix_height: 5496000,
+    plot_filter_128_height: 10542000,
+    plot_filter_64_height: 15592000,
+    plot_filter_32_height: 20643000,
+};
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/error.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/fast_forward.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/fast_forward.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/coin_id.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/coin_id.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/condition_sanitizers.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/condition_sanitizers.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/conditions.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/conditions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     ASSERT_PUZZLE_ANNOUNCEMENT, ASSERT_SECONDS_ABSOLUTE, ASSERT_SECONDS_RELATIVE, CREATE_COIN,
     CREATE_COIN_ANNOUNCEMENT, CREATE_COIN_COST, CREATE_PUZZLE_ANNOUNCEMENT, RECEIVE_MESSAGE,
     REMARK, RESERVE_FEE, SEND_MESSAGE, SOFTFORK,
 };
 use super::sanitize_int::{sanitize_uint, SanitizedUint};
 use super::validation_error::{first, next, rest, ErrorCode, ValidationErr};
 use crate::gen::flags::{
-    AGG_SIG_ARGS, COND_ARGS_NIL, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS,
-    STRICT_ARGS_COUNT,
+    AGG_SIG_ARGS, COND_ARGS_NIL, DISALLOW_INFINITY_G1, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
+    NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
 };
 use crate::gen::messages::{Message, SpendId};
 use crate::gen::spend_visitor::SpendVisitor;
 use crate::gen::validation_error::check_nil;
+use chia_bls::PublicKey;
 use chia_protocol::Bytes32;
 use clvmr::allocator::{Allocator, NodePtr, SExp};
 use clvmr::cost::Cost;
 use clvmr::sha2::{Digest, Sha256};
 use std::cmp::{max, min};
 use std::collections::{HashMap, HashSet};
 use std::hash::{Hash, Hasher};
@@ -663,21 +664,21 @@
     // all coins created by this spend. Duplicates are consensus failures
     // if the coin is asserting its birth height or timestamp, these are set
     pub birth_height: Option<u32>,
     pub birth_seconds: Option<u64>,
     pub create_coin: HashSet<NewCoin>,
     // Agg Sig Me conditions
     // Maybe this should be an array of vectors
-    pub agg_sig_me: Vec<(NodePtr, NodePtr)>,
-    pub agg_sig_parent: Vec<(NodePtr, NodePtr)>,
-    pub agg_sig_puzzle: Vec<(NodePtr, NodePtr)>,
-    pub agg_sig_amount: Vec<(NodePtr, NodePtr)>,
-    pub agg_sig_puzzle_amount: Vec<(NodePtr, NodePtr)>,
-    pub agg_sig_parent_amount: Vec<(NodePtr, NodePtr)>,
-    pub agg_sig_parent_puzzle: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_me: Vec<(PublicKey, NodePtr)>,
+    pub agg_sig_parent: Vec<(PublicKey, NodePtr)>,
+    pub agg_sig_puzzle: Vec<(PublicKey, NodePtr)>,
+    pub agg_sig_amount: Vec<(PublicKey, NodePtr)>,
+    pub agg_sig_puzzle_amount: Vec<(PublicKey, NodePtr)>,
+    pub agg_sig_parent_amount: Vec<(PublicKey, NodePtr)>,
+    pub agg_sig_parent_puzzle: Vec<(PublicKey, NodePtr)>,
     // Flags describing properties of this spend. See flags above
     pub flags: u32,
 }
 
 impl Spend {
     pub fn new(
         parent_id: NodePtr,
@@ -723,15 +724,15 @@
     // ignored. 0 (or negative values) are not passed up to the next layer
     // The sum of all reserve fee conditions
     pub reserve_fee: u64,
     // the highest height/time conditions (i.e. most strict). 0 values are no-ops
     pub height_absolute: u32,
     pub seconds_absolute: u64,
     // Unsafe Agg Sig conditions (i.e. not tied to the spend generating it)
-    pub agg_sig_unsafe: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_unsafe: Vec<(PublicKey, NodePtr)>,
     // when set, this is the lowest (i.e. most restrictive) of all
     // ASSERT_BEFORE_HEIGHT_ABSOLUTE conditions
     pub before_height_absolute: Option<u32>,
     // ASSERT_BEFORE_SECONDS_ABSOLUTE conditions
     pub before_seconds_absolute: Option<u64>,
 
     // the cost of conditions (when returned by parse_spends())
@@ -886,14 +887,28 @@
         Err(ValidationErr(n, ErrorCode::TooManyAnnouncements))
     } else {
         *cnt -= 1;
         Ok(())
     }
 }
 
+fn to_key(a: &Allocator, pk: NodePtr, flags: u32) -> Result<Option<PublicKey>, ValidationErr> {
+    let key = PublicKey::from_bytes(a.atom(pk).as_ref().try_into().expect("internal error"))
+        .map_err(|_| ValidationErr(pk, ErrorCode::InvalidPublicKey))?;
+    if key.is_inf() {
+        if (flags & DISALLOW_INFINITY_G1) != 0 {
+            Err(ValidationErr(pk, ErrorCode::InvalidPublicKey))
+        } else {
+            Ok(None)
+        }
+    } else {
+        Ok(Some(key))
+    }
+}
+
 #[allow(clippy::too_many_arguments)]
 pub fn parse_conditions<V: SpendVisitor>(
     a: &Allocator,
     ret: &mut SpendBundleConditions,
     state: &mut ParseState,
     mut spend: Spend,
     mut iter: NodePtr,
@@ -1128,36 +1143,52 @@
                 state.assert_concurrent_spend.insert(id);
             }
             Condition::AssertConcurrentPuzzle(id) => {
                 decrement(&mut announce_countdown, id)?;
                 state.assert_concurrent_puzzle.insert(id);
             }
             Condition::AggSigMe(pk, msg) => {
-                spend.agg_sig_me.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_me.push((pk, msg));
+                }
             }
             Condition::AggSigParent(pk, msg) => {
-                spend.agg_sig_parent.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_parent.push((pk, msg));
+                }
             }
             Condition::AggSigPuzzle(pk, msg) => {
-                spend.agg_sig_puzzle.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_puzzle.push((pk, msg));
+                }
             }
             Condition::AggSigAmount(pk, msg) => {
-                spend.agg_sig_amount.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_amount.push((pk, msg));
+                }
             }
             Condition::AggSigPuzzleAmount(pk, msg) => {
-                spend.agg_sig_puzzle_amount.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_puzzle_amount.push((pk, msg));
+                }
             }
             Condition::AggSigParentAmount(pk, msg) => {
-                spend.agg_sig_parent_amount.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_parent_amount.push((pk, msg));
+                }
             }
             Condition::AggSigParentPuzzle(pk, msg) => {
-                spend.agg_sig_parent_puzzle.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    spend.agg_sig_parent_puzzle.push((pk, msg));
+                }
             }
             Condition::AggSigUnsafe(pk, msg) => {
-                ret.agg_sig_unsafe.push((pk, msg));
+                if let Some(pk) = to_key(a, pk, flags)? {
+                    ret.agg_sig_unsafe.push((pk, msg));
+                }
             }
             Condition::Softfork(cost) => {
                 if *max_cost < cost {
                     return Err(ValidationErr(c, ErrorCode::CostExceeded));
                 }
                 *max_cost -= cost;
             }
@@ -1459,14 +1490,16 @@
 #[cfg(test)]
 use clvmr::number::Number;
 #[cfg(test)]
 use clvmr::serde::node_to_bytes;
 #[cfg(test)]
 use hex::FromHex;
 #[cfg(test)]
+use hex_literal::hex;
+#[cfg(test)]
 use num_traits::Num;
 #[cfg(test)]
 use rstest::rstest;
 
 #[cfg(test)]
 const H1: &[u8; 32] = &[
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
@@ -1479,18 +1512,15 @@
 #[cfg(test)]
 const LONG_VEC: &[u8; 33] = &[
     3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
     3,
 ];
 
 #[cfg(test)]
-const PUBKEY: &[u8; 48] = &[
-    6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6,
-    6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 6,
-];
+const PUBKEY: &[u8; 48] = &hex!("97f1d3a73197d7942695638c4fa9ac0fc3688c4f9774b905a14e3a3f171bac586c55e83ff97a1aeffb3af00adb22c6bb");
 #[cfg(test)]
 const MSG1: &[u8; 13] = &[3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3];
 #[cfg(test)]
 const MSG2: &[u8; 19] = &[4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4];
 
 #[cfg(test)]
 const LONGMSG: &[u8; 1025] = &[
@@ -2984,15 +3014,15 @@
             .unwrap_err()
             .1,
         ErrorCode::DuplicateOutput
     );
 }
 
 #[cfg(test)]
-fn agg_sig_vec(c: ConditionOpcode, s: &Spend) -> &[(NodePtr, NodePtr)] {
+fn agg_sig_vec(c: ConditionOpcode, s: &Spend) -> &[(PublicKey, NodePtr)] {
     match c {
         AGG_SIG_ME => &s.agg_sig_me,
         AGG_SIG_PARENT => &s.agg_sig_parent,
         AGG_SIG_PUZZLE => &s.agg_sig_puzzle,
         AGG_SIG_AMOUNT => &s.agg_sig_amount,
         AGG_SIG_PUZZLE_AMOUNT => &s.agg_sig_puzzle_amount,
         AGG_SIG_PARENT_AMOUNT => &s.agg_sig_parent_amount,
@@ -3032,15 +3062,15 @@
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
 
     let agg_sigs = agg_sig_vec(condition, spend);
     assert_eq!(agg_sigs.len(), 1);
     for c in agg_sigs {
-        assert_eq!(a.atom(c.0).as_ref(), PUBKEY);
+        assert_eq!(c.0, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(c.1).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[cfg(test)]
 #[rstest]
@@ -3069,29 +3099,30 @@
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
 
     let agg_sigs = agg_sig_vec(condition, spend);
     assert_eq!(agg_sigs.len(), 2);
     for c in agg_sigs {
-        assert_eq!(a.atom(c.0).as_ref(), PUBKEY);
+        assert_eq!(c.0, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(c.1).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(AGG_SIG_ME)]
 #[case(AGG_SIG_PARENT)]
 #[case(AGG_SIG_PUZZLE)]
 #[case(AGG_SIG_AMOUNT)]
 #[case(AGG_SIG_PUZZLE_AMOUNT)]
 #[case(AGG_SIG_PARENT_PUZZLE)]
 #[case(AGG_SIG_PARENT_AMOUNT)]
+#[case(AGG_SIG_UNSAFE)]
 fn test_agg_sig_invalid_pubkey(
     #[case] condition: ConditionOpcode,
     #[values(MEMPOOL_MODE, 0)] mempool: u32,
 ) {
     assert_eq!(
         cond_test_flag(
             &format!(
@@ -3111,14 +3142,53 @@
 #[case(AGG_SIG_ME)]
 #[case(AGG_SIG_PARENT)]
 #[case(AGG_SIG_PUZZLE)]
 #[case(AGG_SIG_AMOUNT)]
 #[case(AGG_SIG_PUZZLE_AMOUNT)]
 #[case(AGG_SIG_PARENT_PUZZLE)]
 #[case(AGG_SIG_PARENT_AMOUNT)]
+#[case(AGG_SIG_UNSAFE)]
+fn test_agg_sig_infinity_pubkey(
+    #[case] condition: ConditionOpcode,
+    #[values(DISALLOW_INFINITY_G1, 0)] mempool: u32,
+) {
+    let ret = cond_test_flag(
+        &format!(
+            "((({{h1}} ({{h2}} (123 ((({} (0xc00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 ({{msg1}} )))))",
+            condition as u8
+            ),
+            ENABLE_SOFTFORK_CONDITION | mempool
+    );
+
+    if mempool != 0 {
+        assert_eq!(ret.unwrap_err().1, ErrorCode::InvalidPublicKey);
+    } else {
+        let ret = ret.expect("expected conditions to be valid").1;
+        assert!(ret.agg_sig_unsafe.is_empty());
+        for c in ret.spends {
+            assert!(c.agg_sig_me.is_empty());
+            assert!(c.agg_sig_parent.is_empty());
+            assert!(c.agg_sig_puzzle.is_empty());
+            assert!(c.agg_sig_amount.is_empty());
+            assert!(c.agg_sig_puzzle_amount.is_empty());
+            assert!(c.agg_sig_parent_amount.is_empty());
+            assert!(c.agg_sig_parent_puzzle.is_empty());
+        }
+    }
+}
+
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
 fn test_agg_sig_invalid_msg(
     #[case] condition: ConditionOpcode,
     #[values(MEMPOOL_MODE, 0)] mempool: u32,
 ) {
     assert_eq!(
         cond_test_flag(
             &format!(
@@ -3184,15 +3254,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(*pk, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_extra_arg() {
@@ -3277,15 +3347,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(*pk, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_me_extra_arg_allowed() {
@@ -3302,15 +3372,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 1);
     for c in &spend.agg_sig_me {
-        assert_eq!(a.atom(c.0).as_ref(), PUBKEY);
+        assert_eq!(c.0, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(c.1).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_terminator() {
@@ -3324,15 +3394,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(*pk, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_terminator_mempool() {
@@ -3361,15 +3431,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(spend.agg_sig_me.len(), 1);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(*pk, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_me_invalid_terminator_mempool() {
@@ -3400,15 +3470,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash).as_ref(), H2);
     assert_eq!(conds.agg_sig_unsafe.len(), 2);
     for (pk, msg) in &conds.agg_sig_unsafe {
-        assert_eq!(a.atom(*pk).as_ref(), PUBKEY);
+        assert_eq!(*pk, PublicKey::from_bytes(PUBKEY).unwrap());
         assert_eq!(a.atom(*msg).as_ref(), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_pubkey() {
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/flags.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/flags.rs`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,21 @@
 // When set, the "flags" field of the Spend objects will be set depending on
 // what features are detected of the spends
 pub const ANALYZE_SPENDS: u32 = 0x4000000;
 
 // This enables support for the new SEND_MESSAGE and RECEIVE_MESSAGE conditions
 pub const ENABLE_MESSAGE_CONDITIONS: u32 = 0x8000000;
 
+// When this flag is set, we reject AGG_SIG_* conditions whose public key is the
+// infinity G1 point. Such public keys are mathematically valid, but do not
+// provide any security guarantees. Chia has historically allowed them. Enabling
+// this flag is a soft-fork.
+pub const DISALLOW_INFINITY_G1: u32 = 0x10000000;
+
 pub const MEMPOOL_MODE: u32 = CLVM_MEMPOOL_MODE
     | NO_UNKNOWN_CONDS
     | COND_ARGS_NIL
     | STRICT_ARGS_COUNT
     | NO_RELATIVE_CONDITIONS_ON_EPHEMERAL
     | ANALYZE_SPENDS
-    | ENABLE_MESSAGE_CONDITIONS;
+    | ENABLE_MESSAGE_CONDITIONS
+    | DISALLOW_INFINITY_G1;
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/get_puzzle_and_solution.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/get_puzzle_and_solution.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/messages.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/messages.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/opcodes.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/opcodes.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/owned_conditions.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/owned_conditions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -108,18 +108,15 @@
         let mut spends = Vec::<OwnedSpend>::new();
         for s in sb.spends {
             spends.push(OwnedSpend::from(a, s)?);
         }
 
         let mut agg_sigs = Vec::<(PublicKey, Bytes)>::with_capacity(sb.agg_sig_unsafe.len());
         for (pk, msg) in sb.agg_sig_unsafe {
-            agg_sigs.push((
-                PublicKey::from_bytes(a.atom(pk).as_ref().try_into().unwrap())?,
-                a.atom(msg).as_ref().into(),
-            ));
+            agg_sigs.push((pk, a.atom(msg).as_ref().into()));
         }
 
         Ok(Self {
             spends,
             reserve_fee: sb.reserve_fee,
             height_absolute: sb.height_absolute,
             seconds_absolute: sb.seconds_absolute,
@@ -131,18 +128,15 @@
             addition_amount: sb.addition_amount,
         })
     }
 }
 
 fn convert_agg_sigs(
     a: &Allocator,
-    agg_sigs: &[(NodePtr, NodePtr)],
+    agg_sigs: &[(PublicKey, NodePtr)],
 ) -> Result<Vec<(PublicKey, Bytes)>> {
     let mut ret = Vec::<(PublicKey, Bytes)>::new();
     for (pk, msg) in agg_sigs {
-        ret.push((
-            PublicKey::from_bytes(a.atom(*pk).as_ref().try_into().unwrap())?,
-            a.atom(*msg).as_ref().into(),
-        ));
+        ret.push((*pk, a.atom(*msg).as_ref().into()));
     }
     Ok(ret)
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/run_block_generator.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/run_block_generator.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/run_puzzle.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/run_puzzle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/sanitize_int.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/sanitize_int.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/solution_generator.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/solution_generator.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/test_generators.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/test_generators.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,15 @@
         ret += &format!("ASSERT_BEFORE_SECONDS_ABSOLUTE {val}\n");
     }
     if let Some(val) = c.before_height_absolute {
         ret += &format!("ASSERT_BEFORE_HEIGHT_ABSOLUTE {val}\n");
     }
     let mut agg_sigs = Vec::<(Bytes48, Bytes)>::new();
     for (pk, msg) in &c.agg_sig_unsafe {
-        agg_sigs.push((
-            a.atom(*pk).as_ref().try_into().unwrap(),
-            a.atom(*msg).as_ref().into(),
-        ));
+        agg_sigs.push((pk.to_bytes().into(), a.atom(*msg).as_ref().into()));
     }
     agg_sigs.sort();
     for (pk, msg) in agg_sigs {
         ret += &format!(
             "AGG_SIG_UNSAFE pk: {} msg: {}\n",
             hex::encode(pk),
             hex::encode(msg)
@@ -84,18 +81,15 @@
                     cc.amount
                 );
             }
         }
 
         let mut agg_sigs = Vec::<(Bytes48, Bytes)>::new();
         for (pk, msg) in s.agg_sig_me {
-            agg_sigs.push((
-                a.atom(pk).as_ref().try_into().unwrap(),
-                a.atom(msg).as_ref().into(),
-            ));
+            agg_sigs.push((pk.to_bytes().into(), a.atom(msg).as_ref().into()));
         }
         agg_sigs.sort();
         for (pk, msg) in agg_sigs {
             ret += &format!(
                 "  AGG_SIG_ME pk: {} msg: {}\n",
                 hex::encode(pk),
                 hex::encode(msg)
@@ -145,14 +139,15 @@
                 println!("\x1b[0m");
             }
         }
     }
 }
 
 #[rstest]
+#[case("infinity-g1")]
 #[case("block-1ee588dc")]
 #[case("block-6fe59b24")]
 #[case("block-b45268ac")]
 #[case("block-c2a8df0d")]
 #[case("block-e5002df2")]
 #[case("block-4671894")]
 #[case("block-225758")]
```

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/gen/validation_error.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/gen/validation_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/generator_rom.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/generator_rom.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/merkle_set.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/merkle_set.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-consensus/src/merkle_tree.rs` & `chia_rs-0.9.0/crates/chia-consensus/src/merkle_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -348,39 +348,39 @@
     Ok(tree.generate_proof(item)?.0)
 }
 
 #[cfg(feature = "py-bindings")]
 #[pymethods]
 impl MerkleSet {
     #[new]
-    pub fn init(leafs: &PyList) -> PyResult<Self> {
+    pub fn init(leafs: &Bound<PyList>) -> PyResult<Self> {
         let mut data: Vec<[u8; 32]> = Vec::with_capacity(leafs.len());
 
         for leaf in leafs {
             data.push(
                 leaf.extract::<[u8; 32]>()
                     .map_err(|_| PyValueError::new_err("invalid leaf"))?,
             );
         }
         Ok(MerkleSet::from_leafs(&mut data))
     }
 
     #[pyo3(name = "get_root")]
-    pub fn py_get_root<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
+    pub fn py_get_root<'a>(&self, py: Python<'a>) -> PyResult<Bound<'a, PyAny>> {
         ChiaToPython::to_python(&Bytes32::new(self.get_root()), py)
     }
 
     #[pyo3(name = "is_included_already_hashed")]
     pub fn py_generate_proof(
         &self,
         py: Python,
         included_leaf: [u8; 32],
     ) -> PyResult<(bool, PyObject)> {
         match self.generate_proof(&included_leaf) {
-            Ok((included, proof)) => Ok((included, PyBytes::new(py, &proof).into())),
+            Ok((included, proof)) => Ok((included, PyBytes::new_bound(py, &proof).into())),
             Err(_) => Err(PyValueError::new_err("invalid proof")),
         }
     }
 }
 
 impl From<ArrayTypes> for NodeType {
     fn from(val: ArrayTypes) -> NodeType {
@@ -640,17 +640,17 @@
             assert_eq!(new_proof, Vec::<u8>::new());
             assert_eq!(rebuilt.get_root(), root);
         }
     }
 
     // these tests take a long time to run in unoptimized builds.
     #[cfg(not(debug_assertions))]
-    const TEST_ITERS: i32 = 10000;
+    const TEST_ITERS: i32 = 1000;
     #[cfg(debug_assertions)]
-    const TEST_ITERS: i32 = 400;
+    const TEST_ITERS: i32 = 300;
 
     // this test generates a random tree and ensures we can produce the tree
     // with the correct root hash and that we can generate proofs, and validate
     // them, for every item
     #[test]
     fn test_random_bytes() {
         let mut rng = SmallRng::seed_from_u64(1337);
```

### Comparing `chia_rs-0.8.0/crates/clvm-traits/Cargo.toml` & `chia_rs-0.9.0/crates/clvm-traits/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "clvm-traits"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Traits for encoding and decoding CLVM objects."
 authors = ["Brandon Haggstrom <b.haggstrom@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 
@@ -13,17 +13,17 @@
 
 [features]
 derive = ["dep:clvm-derive"]
 chia-bls = ["dep:chia-bls"]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
-pyo3 = { version = ">=0.19.0", optional = true }
+pyo3 = { version = "0.21.2", optional = true }
 clvmr = "0.7.0"
-clvm-derive = { version = "0.6.0", path = "../clvm-derive", optional = true }
-chia-bls = { version = "0.8.0", path = "../chia-bls", optional = true }
+clvm-derive = { version = "0.9.0", path = "../clvm-derive", optional = true }
+chia-bls = { version = "0.9.0", path = "../chia-bls", optional = true }
 num-bigint = "0.4.3"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 hex = "0.4.3"
 hex-literal = "0.4.1"
```

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/clvm_decoder.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/clvm_decoder.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 use clvmr::{allocator::SExp, Allocator, Atom, NodePtr};
 
-use crate::{FromClvm, FromClvmError};
+use crate::{
+    destructure_list, destructure_quote, match_list, match_quote, FromClvm, FromClvmError,
+    MatchByte,
+};
 
-pub trait ClvmDecoder {
-    type Node: Clone;
+pub trait ClvmDecoder: Sized {
+    type Node: Clone + FromClvm<Self::Node>;
 
     fn decode_atom(&self, node: &Self::Node) -> Result<Atom, FromClvmError>;
     fn decode_pair(&self, node: &Self::Node) -> Result<(Self::Node, Self::Node), FromClvmError>;
 
+    fn decode_curried_arg(
+        &self,
+        node: &Self::Node,
+    ) -> Result<(Self::Node, Self::Node), FromClvmError> {
+        let destructure_list!(_, destructure_quote!(first), rest) =
+            <match_list!(MatchByte<4>, match_quote!(Self::Node), Self::Node)>::from_clvm(
+                self,
+                node.clone(),
+            )?;
+        Ok((first, rest))
+    }
+
     /// This is a helper function that just calls `clone` on the node.
     /// It's required only because the compiler can't infer that `N` is `Clone`,
     /// since there's no `Clone` bound on the `FromClvm` trait.
     fn clone_node(&self, node: &Self::Node) -> Self::Node {
         node.clone()
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/clvm_encoder.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/clvm_encoder.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 use clvmr::{Allocator, NodePtr};
 
-use crate::{ToClvm, ToClvmError};
+use crate::{clvm_list, clvm_quote, ToClvm, ToClvmError};
 
-pub trait ClvmEncoder {
-    type Node: Clone;
+pub trait ClvmEncoder: Sized {
+    type Node: Clone + ToClvm<Self::Node>;
 
     fn encode_atom(&mut self, bytes: &[u8]) -> Result<Self::Node, ToClvmError>;
     fn encode_pair(
         &mut self,
         first: Self::Node,
         rest: Self::Node,
     ) -> Result<Self::Node, ToClvmError>;
 
+    fn encode_curried_arg(
+        &mut self,
+        first: Self::Node,
+        rest: Self::Node,
+    ) -> Result<Self::Node, ToClvmError> {
+        const OP_C: u8 = 4;
+        clvm_list!(OP_C, clvm_quote!(first), rest).to_clvm(self)
+    }
+
     /// This is a helper function that just calls `clone` on the node.
     /// It's required only because the compiler can't infer that `N` is `Clone`,
     /// since there's no `Clone` bound on the `ToClvm` trait.
     fn clone_node(&self, node: &Self::Node) -> Self::Node {
         node.clone()
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/error.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/from_clvm.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/from_clvm.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/macros.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/match_byte.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/match_byte.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/to_clvm.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/to_clvm.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/clvm-traits/src/wrappers.rs` & `chia_rs-0.9.0/crates/clvm-traits/src/wrappers.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/Cargo.toml` & `chia_rs-0.9.0/crates/chia-puzzles/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chia-puzzles"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chia primitives needed for building wallets."
 authors = ["Brandon Haggstrom <b.haggstrom@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 
@@ -12,18 +12,18 @@
 arbitrary = ["dep:arbitrary", "chia-protocol/arbitrary"]
 
 [dependencies]
 clvmr = "0.7.0"
 sha2 = "0.10.8"
 num-bigint = "0.4.3"
 hex-literal = "0.4.1"
-clvm-utils = { version = "0.8.0", path = "../clvm-utils" }
-clvm-traits = { version = "0.8.0", path = "../clvm-traits", features = ["chia-bls"] }
-chia-bls = { version = "0.8.0", path = "../chia-bls" }
-chia-protocol = { version = "0.8.0", path = "../chia-protocol" }
+clvm-utils = { version = "0.9.0", path = "../clvm-utils" }
+clvm-traits = { version = "0.9.0", path = "../clvm-traits", features = ["chia-bls"] }
+chia-bls = { version = "0.9.0", path = "../chia-bls" }
+chia-protocol = { version = "0.9.0", path = "../chia-protocol" }
 arbitrary = { version = "1.3.0", features = ["derive"], optional = true }
 
 [dev-dependencies]
 hex = "0.4.3"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/derive_synthetic.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/derive_synthetic.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/proof.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/proof.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use chia_protocol::Bytes32;
 use clvm_traits::{FromClvm, ToClvm};
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
-#[clvm(untagged, tuple)]
+#[clvm(transparent)]
 pub enum Proof {
     Lineage(LineageProof),
     Eve(EveProof),
 }
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
```

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/cat.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/cat.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,90 @@
 use chia_bls::PublicKey;
 use chia_protocol::{Bytes32, Coin};
 use clvm_traits::{FromClvm, ToClvm};
-use clvm_utils::TreeHash;
+use clvm_utils::{CurriedProgram, ToTreeHash, TreeHash};
 use hex_literal::hex;
 
 use crate::LineageProof;
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct CatArgs<I> {
     pub mod_hash: Bytes32,
-    pub tail_program_hash: Bytes32,
+    pub asset_id: Bytes32,
     pub inner_puzzle: I,
 }
 
+impl<I> CatArgs<I> {
+    pub fn new(asset_id: Bytes32, inner_puzzle: I) -> Self {
+        Self {
+            mod_hash: CAT_PUZZLE_HASH.into(),
+            asset_id,
+            inner_puzzle,
+        }
+    }
+}
+
+impl CatArgs<TreeHash> {
+    pub fn curry_tree_hash(asset_id: Bytes32, inner_puzzle: TreeHash) -> TreeHash {
+        CurriedProgram {
+            program: CAT_PUZZLE_HASH,
+            args: CatArgs {
+                mod_hash: CAT_PUZZLE_HASH.into(),
+                asset_id,
+                inner_puzzle,
+            },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct EverythingWithSignatureTailArgs {
     pub public_key: PublicKey,
 }
 
+impl EverythingWithSignatureTailArgs {
+    pub fn new(public_key: PublicKey) -> Self {
+        Self { public_key }
+    }
+
+    pub fn curry_tree_hash(public_key: PublicKey) -> TreeHash {
+        CurriedProgram {
+            program: EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE_HASH,
+            args: EverythingWithSignatureTailArgs { public_key },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct GenesisByCoinIdTailArgs {
     pub genesis_coin_id: Bytes32,
 }
 
+impl GenesisByCoinIdTailArgs {
+    pub fn new(genesis_coin_id: Bytes32) -> Self {
+        Self { genesis_coin_id }
+    }
+
+    pub fn curry_tree_hash(genesis_coin_id: Bytes32) -> TreeHash {
+        CurriedProgram {
+            program: GENESIS_BY_COIN_ID_TAIL_PUZZLE_HASH,
+            args: GenesisByCoinIdTailArgs { genesis_coin_id },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(list)]
 pub struct CatSolution<I> {
     pub inner_puzzle_solution: I,
     pub lineage_proof: Option<LineageProof>,
     pub prev_coin_id: Bytes32,
@@ -214,121 +266,97 @@
     72dec062874cd4d3aab892a0906688a1ae412b0109982e1797a170add88bdcdc
     "
 ));
 
 #[cfg(test)]
 mod tests {
     use clvm_traits::ToNodePtr;
-    use clvm_utils::{tree_hash, CurriedProgram, ToTreeHash};
+    use clvm_utils::tree_hash;
     use clvmr::{serde::node_from_bytes, Allocator};
 
     use super::*;
 
     use crate::{
         assert_puzzle_hash,
-        standard::{StandardArgs, STANDARD_PUZZLE, STANDARD_PUZZLE_HASH},
+        standard::{StandardArgs, STANDARD_PUZZLE},
     };
 
     #[test]
     fn puzzle_hashes() {
         assert_puzzle_hash!(CAT_PUZZLE => CAT_PUZZLE_HASH);
         assert_puzzle_hash!(CAT_PUZZLE_V1 => CAT_PUZZLE_HASH_V1);
         assert_puzzle_hash!(EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE => EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE_HASH);
         assert_puzzle_hash!(GENESIS_BY_COIN_ID_TAIL_PUZZLE => GENESIS_BY_COIN_ID_TAIL_PUZZLE_HASH);
     }
 
     #[test]
     fn curry_cat_tree_hash() {
-        let inner_args = StandardArgs {
-            synthetic_key: PublicKey::default(),
-        };
+        let synthetic_key = PublicKey::default();
         let asset_id = Bytes32::new([120; 32]);
 
         let mut a = Allocator::new();
         let mod_ptr = node_from_bytes(&mut a, &CAT_PUZZLE).unwrap();
         let inner_mod_ptr = node_from_bytes(&mut a, &STANDARD_PUZZLE).unwrap();
+
         let curried_ptr = CurriedProgram {
             program: mod_ptr,
-            args: CatArgs {
-                mod_hash: CAT_PUZZLE_HASH.into(),
-                inner_puzzle: CurriedProgram {
+            args: CatArgs::new(
+                asset_id,
+                CurriedProgram {
                     program: inner_mod_ptr,
-                    args: &inner_args,
+                    args: StandardArgs::new(synthetic_key),
                 },
-                tail_program_hash: asset_id,
-            },
+            ),
         }
         .to_node_ptr(&mut a)
         .unwrap();
 
         let allocated_tree_hash = hex::encode(tree_hash(&a, curried_ptr));
 
-        let tree_hash = hex::encode(
-            CurriedProgram {
-                program: CAT_PUZZLE_HASH,
-                args: CatArgs {
-                    mod_hash: CAT_PUZZLE_HASH.into(),
-                    inner_puzzle: CurriedProgram {
-                        program: STANDARD_PUZZLE_HASH,
-                        args: &inner_args,
-                    },
-                    tail_program_hash: asset_id,
-                },
-            }
-            .tree_hash(),
-        );
+        let inner_puzzle_hash = StandardArgs::curry_tree_hash(synthetic_key);
+        let tree_hash = hex::encode(CatArgs::curry_tree_hash(asset_id, inner_puzzle_hash));
 
         assert_eq!(allocated_tree_hash, tree_hash);
     }
 
     #[test]
     fn curry_everything_with_signature() {
         let public_key = PublicKey::default();
 
         let mut a = Allocator::new();
         let mod_ptr = node_from_bytes(&mut a, &EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE).unwrap();
+
         let curried_ptr = CurriedProgram {
             program: mod_ptr,
-            args: EverythingWithSignatureTailArgs { public_key },
+            args: EverythingWithSignatureTailArgs::new(public_key),
         }
         .to_node_ptr(&mut a)
         .unwrap();
 
         let allocated_tree_hash = hex::encode(tree_hash(&a, curried_ptr));
 
-        let tree_hash = hex::encode(
-            CurriedProgram {
-                program: EVERYTHING_WITH_SIGNATURE_TAIL_PUZZLE_HASH,
-                args: EverythingWithSignatureTailArgs { public_key },
-            }
-            .tree_hash(),
-        );
+        let tree_hash = hex::encode(EverythingWithSignatureTailArgs::curry_tree_hash(public_key));
 
         assert_eq!(allocated_tree_hash, tree_hash);
     }
 
     #[test]
     fn curry_genesis_by_coin_id() {
         let genesis_coin_id = Bytes32::new([120; 32]);
 
         let mut a = Allocator::new();
         let mod_ptr = node_from_bytes(&mut a, &GENESIS_BY_COIN_ID_TAIL_PUZZLE).unwrap();
+
         let curried_ptr = CurriedProgram {
             program: mod_ptr,
-            args: GenesisByCoinIdTailArgs { genesis_coin_id },
+            args: GenesisByCoinIdTailArgs::new(genesis_coin_id),
         }
         .to_node_ptr(&mut a)
         .unwrap();
 
         let allocated_tree_hash = hex::encode(tree_hash(&a, curried_ptr));
 
-        let tree_hash = hex::encode(
-            CurriedProgram {
-                program: GENESIS_BY_COIN_ID_TAIL_PUZZLE_HASH,
-                args: GenesisByCoinIdTailArgs { genesis_coin_id },
-            }
-            .tree_hash(),
-        );
+        let tree_hash = hex::encode(GenesisByCoinIdTailArgs::curry_tree_hash(genesis_coin_id));
 
         assert_eq!(allocated_tree_hash, tree_hash);
     }
 }
```

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/did.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/did.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/nft.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/nft.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,81 @@
 use chia_protocol::Bytes32;
 use clvm_traits::{ClvmDecoder, ClvmEncoder, FromClvm, FromClvmError, Raw, ToClvm, ToClvmError};
-use clvm_utils::TreeHash;
+use clvm_utils::{CurriedProgram, ToTreeHash, TreeHash};
 use hex_literal::hex;
 
-use crate::singleton::SingletonStruct;
+use crate::singleton::{SingletonStruct, SINGLETON_LAUNCHER_PUZZLE_HASH};
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct NftIntermediateLauncherArgs {
     pub launcher_puzzle_hash: Bytes32,
     pub mint_number: usize,
     pub mint_total: usize,
 }
 
+impl NftIntermediateLauncherArgs {
+    pub fn new(mint_number: usize, mint_total: usize) -> Self {
+        Self {
+            launcher_puzzle_hash: SINGLETON_LAUNCHER_PUZZLE_HASH.into(),
+            mint_number,
+            mint_total,
+        }
+    }
+
+    pub fn curry_tree_hash(mint_number: usize, mint_total: usize) -> TreeHash {
+        CurriedProgram {
+            program: NFT_INTERMEDIATE_LAUNCHER_PUZZLE_HASH,
+            args: NftIntermediateLauncherArgs {
+                launcher_puzzle_hash: SINGLETON_LAUNCHER_PUZZLE_HASH.into(),
+                mint_number,
+                mint_total,
+            },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct NftStateLayerArgs<I, M> {
     pub mod_hash: Bytes32,
     pub metadata: M,
     pub metadata_updater_puzzle_hash: Bytes32,
     pub inner_puzzle: I,
 }
 
+impl<I, M> NftStateLayerArgs<I, M> {
+    pub fn new(metadata: M, inner_puzzle: I) -> Self {
+        Self {
+            mod_hash: NFT_STATE_LAYER_PUZZLE_HASH.into(),
+            metadata,
+            metadata_updater_puzzle_hash: NFT_METADATA_UPDATER_PUZZLE_HASH.into(),
+            inner_puzzle,
+        }
+    }
+}
+
+impl NftStateLayerArgs<TreeHash, TreeHash> {
+    pub fn curry_tree_hash(metadata: TreeHash, inner_puzzle: TreeHash) -> TreeHash {
+        CurriedProgram {
+            program: NFT_STATE_LAYER_PUZZLE_HASH,
+            args: NftStateLayerArgs {
+                mod_hash: NFT_STATE_LAYER_PUZZLE_HASH.into(),
+                metadata,
+                metadata_updater_puzzle_hash: NFT_METADATA_UPDATER_PUZZLE_HASH.into(),
+                inner_puzzle,
+            },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(list)]
 pub struct NftStateLayerSolution<I> {
     pub inner_solution: I,
 }
 
@@ -37,14 +85,44 @@
 pub struct NftOwnershipLayerArgs<I, P> {
     pub mod_hash: Bytes32,
     pub current_owner: Option<Bytes32>,
     pub transfer_program: P,
     pub inner_puzzle: I,
 }
 
+impl<I, P> NftOwnershipLayerArgs<I, P> {
+    pub fn new(current_owner: Option<Bytes32>, transfer_program: P, inner_puzzle: I) -> Self {
+        Self {
+            mod_hash: NFT_OWNERSHIP_LAYER_PUZZLE_HASH.into(),
+            current_owner,
+            transfer_program,
+            inner_puzzle,
+        }
+    }
+}
+
+impl NftOwnershipLayerArgs<TreeHash, TreeHash> {
+    pub fn curry_tree_hash(
+        current_owner: Option<Bytes32>,
+        transfer_program: TreeHash,
+        inner_puzzle: TreeHash,
+    ) -> TreeHash {
+        CurriedProgram {
+            program: NFT_OWNERSHIP_LAYER_PUZZLE_HASH,
+            args: NftOwnershipLayerArgs {
+                mod_hash: NFT_OWNERSHIP_LAYER_PUZZLE_HASH.into(),
+                current_owner,
+                transfer_program,
+                inner_puzzle,
+            },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(list)]
 pub struct NftOwnershipLayerSolution<I> {
     pub inner_solution: I,
 }
 
@@ -53,14 +131,44 @@
 #[clvm(curry)]
 pub struct NftRoyaltyTransferPuzzleArgs {
     pub singleton_struct: SingletonStruct,
     pub royalty_puzzle_hash: Bytes32,
     pub trade_price_percentage: u16,
 }
 
+impl NftRoyaltyTransferPuzzleArgs {
+    pub fn new(
+        launcher_id: Bytes32,
+        royalty_puzzle_hash: Bytes32,
+        trade_price_percentage: u16,
+    ) -> Self {
+        Self {
+            singleton_struct: SingletonStruct::new(launcher_id),
+            royalty_puzzle_hash,
+            trade_price_percentage,
+        }
+    }
+
+    pub fn curry_tree_hash(
+        launcher_id: Bytes32,
+        royalty_puzzle_hash: Bytes32,
+        trade_price_percentage: u16,
+    ) -> TreeHash {
+        CurriedProgram {
+            program: NFT_ROYALTY_TRANSFER_PUZZLE_HASH,
+            args: NftRoyaltyTransferPuzzleArgs {
+                singleton_struct: SingletonStruct::new(launcher_id),
+                royalty_puzzle_hash,
+                trade_price_percentage,
+            },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, PartialEq, Eq)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 pub struct NftMetadata {
     pub edition_number: u64,
     pub edition_total: u64,
     pub data_uris: Vec<String>,
     pub data_hash: Option<Bytes32>,
```

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/offer.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/offer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 use chia_protocol::{Bytes, Bytes32};
 use clvm_traits::{FromClvm, ToClvm};
 use clvm_utils::TreeHash;
 use hex_literal::hex;
 
 #[derive(Debug, Clone, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
-#[clvm(tuple)]
+#[clvm(transparent)]
 pub struct SettlementPaymentsSolution {
     pub notarized_payments: Vec<NotarizedPayment>,
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
-#[clvm(tuple)]
+#[clvm(list)]
 pub struct NotarizedPayment {
     pub nonce: Bytes32,
+    #[clvm(rest)]
     pub payments: Vec<Payment>,
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
-#[clvm(tuple, untagged)]
+#[clvm(transparent)]
 pub enum Payment {
     WithoutMemos(PaymentWithoutMemos),
     WithMemos(PaymentWithMemos),
 }
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
```

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/singleton.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/singleton.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,64 @@
 use chia_protocol::Bytes32;
 use clvm_traits::{FromClvm, ToClvm};
-use clvm_utils::TreeHash;
+use clvm_utils::{CurriedProgram, ToTreeHash, TreeHash};
 use hex_literal::hex;
 
 use crate::Proof;
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct SingletonArgs<I> {
     pub singleton_struct: SingletonStruct,
     pub inner_puzzle: I,
 }
 
+impl<I> SingletonArgs<I> {
+    pub fn new(launcher_id: Bytes32, inner_puzzle: I) -> Self {
+        Self {
+            singleton_struct: SingletonStruct::new(launcher_id),
+            inner_puzzle,
+        }
+    }
+}
+
+impl SingletonArgs<TreeHash> {
+    pub fn curry_tree_hash(launcher_id: Bytes32, inner_puzzle: TreeHash) -> TreeHash {
+        CurriedProgram {
+            program: SINGLETON_TOP_LAYER_PUZZLE_HASH,
+            args: SingletonArgs {
+                singleton_struct: SingletonStruct::new(launcher_id),
+                inner_puzzle,
+            },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
-#[clvm(tuple)]
+#[clvm(list)]
 pub struct SingletonStruct {
     pub mod_hash: Bytes32,
     pub launcher_id: Bytes32,
+    #[clvm(rest)]
     pub launcher_puzzle_hash: Bytes32,
 }
 
+impl SingletonStruct {
+    pub fn new(launcher_id: Bytes32) -> Self {
+        Self {
+            mod_hash: SINGLETON_TOP_LAYER_PUZZLE_HASH.into(),
+            launcher_id,
+            launcher_puzzle_hash: SINGLETON_LAUNCHER_PUZZLE_HASH.into(),
+        }
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(list)]
 pub struct SingletonSolution<I> {
     pub lineage_proof: Proof,
     pub amount: u64,
     pub inner_solution: I,
@@ -36,24 +69,14 @@
 #[clvm(list)]
 pub struct LauncherSolution<T> {
     pub singleton_puzzle_hash: Bytes32,
     pub amount: u64,
     pub key_value_list: T,
 }
 
-impl SingletonStruct {
-    pub fn new(launcher_id: Bytes32) -> Self {
-        Self {
-            mod_hash: SINGLETON_TOP_LAYER_PUZZLE_HASH.into(),
-            launcher_id,
-            launcher_puzzle_hash: SINGLETON_LAUNCHER_PUZZLE_HASH.into(),
-        }
-    }
-}
-
 /// This is the puzzle reveal of the [singleton launcher](https://chialisp.com/singletons#launcher) puzzle.
 pub const SINGLETON_LAUNCHER_PUZZLE: [u8; 175] = hex!(
     "
     ff02ffff01ff04ffff04ff04ffff04ff05ffff04ff0bff80808080ffff04ffff
     04ff0affff04ffff02ff0effff04ff02ffff04ffff04ff05ffff04ff0bffff04
     ff17ff80808080ff80808080ff808080ff808080ffff04ffff01ff33ff3cff02
     ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff0effff04ff02ffff04ff
```

### Comparing `chia_rs-0.8.0/crates/chia-puzzles/src/puzzles/standard.rs` & `chia_rs-0.9.0/crates/chia-puzzles/src/puzzles/standard.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,53 @@
 use chia_bls::PublicKey;
-use clvm_traits::{FromClvm, ToClvm};
-use clvm_utils::TreeHash;
+use clvm_traits::{clvm_quote, FromClvm, ToClvm};
+use clvm_utils::{CurriedProgram, ToTreeHash, TreeHash};
 use hex_literal::hex;
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(curry)]
 pub struct StandardArgs {
     pub synthetic_key: PublicKey,
 }
 
+impl StandardArgs {
+    pub fn new(synthetic_key: PublicKey) -> Self {
+        Self { synthetic_key }
+    }
+
+    pub fn curry_tree_hash(synthetic_key: PublicKey) -> TreeHash {
+        CurriedProgram {
+            program: STANDARD_PUZZLE_HASH,
+            args: StandardArgs { synthetic_key },
+        }
+        .tree_hash()
+    }
+}
+
 #[derive(Debug, Clone, Copy, PartialEq, Eq, ToClvm, FromClvm)]
 #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[clvm(list)]
 pub struct StandardSolution<P, S> {
     pub original_public_key: Option<PublicKey>,
     pub delegated_puzzle: P,
     pub solution: S,
 }
 
+impl<T> StandardSolution<(u8, T), ()> {
+    /// Outputs the provided condition list directly, without using the hidden puzzle.
+    pub fn from_conditions(conditions: T) -> Self {
+        Self {
+            original_public_key: None,
+            delegated_puzzle: clvm_quote!(conditions),
+            solution: (),
+        }
+    }
+}
+
 /// This is the puzzle reveal of the [standard transaction](https://chialisp.com/standard-transactions) puzzle.
 pub const STANDARD_PUZZLE: [u8; 227] = hex!(
     "
     ff02ffff01ff02ffff03ff0bffff01ff02ffff03ffff09ff05ffff1dff0bffff
     1effff0bff0bffff02ff06ffff04ff02ffff04ff17ff8080808080808080ffff
     01ff02ff17ff2f80ffff01ff088080ff0180ffff01ff04ffff04ff04ffff04ff
     05ffff04ffff02ff06ffff04ff02ffff04ff17ff80808080ff80808080ffff02
@@ -49,48 +74,41 @@
     711d6c4e32c92e53179b199484cf8c897542bc57f2b22582799f9d657eec4699
     "
 ));
 
 #[cfg(test)]
 mod tests {
     use clvm_traits::ToNodePtr;
-    use clvm_utils::{tree_hash, CurriedProgram, ToTreeHash};
+    use clvm_utils::tree_hash;
     use clvmr::{serde::node_from_bytes, Allocator};
 
     use super::*;
 
     use crate::assert_puzzle_hash;
 
     #[test]
     fn puzzle_hashes() {
         assert_puzzle_hash!(STANDARD_PUZZLE => STANDARD_PUZZLE_HASH);
         assert_puzzle_hash!(DEFAULT_HIDDEN_PUZZLE => DEFAULT_HIDDEN_PUZZLE_HASH);
     }
 
     #[test]
     fn curry_tree_hash() {
-        let args = StandardArgs {
-            synthetic_key: PublicKey::default(),
-        };
+        let synthetic_key = PublicKey::default();
 
         let mut a = Allocator::new();
         let mod_ptr = node_from_bytes(&mut a, &STANDARD_PUZZLE).unwrap();
+
         let curried_ptr = CurriedProgram {
             program: mod_ptr,
-            args: &args,
+            args: StandardArgs::new(synthetic_key),
         }
         .to_node_ptr(&mut a)
         .unwrap();
 
         let allocated_tree_hash = hex::encode(tree_hash(&a, curried_ptr));
 
-        let tree_hash = hex::encode(
-            CurriedProgram {
-                program: STANDARD_PUZZLE_HASH,
-                args: &args,
-            }
-            .tree_hash(),
-        );
+        let tree_hash = hex::encode(StandardArgs::curry_tree_hash(synthetic_key));
 
         assert_eq!(allocated_tree_hash, tree_hash);
     }
 }
```

### Comparing `chia_rs-0.8.0/wheel/Cargo.toml` & `chia_rs-0.9.0/wheel/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chia_rs"
-version = "0.8.0"
+version = "0.9.0"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Code useful for implementing chia consensus."
 homepage = "https://github.com/Chia-Network/chia_rs"
 repository = "https://github.com/Chia-Network/chia_rs"
 readme = "README.md"
@@ -14,16 +14,16 @@
 crate-type = ["cdylib"]
 path = "src/lib.rs"
 
 [dependencies]
 clvmr = "0.7.0"
 hex = "0.4.3"
 sha2 = "0.10.8"
-pyo3 = { version = "=0.19.0", features = ["multiple-pymethods"] }
-chia-consensus = { version = "0.8.0", path = "../crates/chia-consensus", features = ["py-bindings"] }
-chia-bls = { version = "0.8.0", path = "../crates/chia-bls", features = ["py-bindings"]  }
-chia-protocol = { version = "0.8.0", path = "../crates/chia-protocol", features = ["py-bindings"]  }
-chia-traits = { version = "0.8.0", path = "../crates/chia-traits", features = ["py-bindings"]  }
-clvm-traits = { version = "0.8.0", path = "../crates/clvm-traits", features = ["derive", "py-bindings"] }
-clvm-utils = { version = "0.8.0", path = "../crates/clvm-utils" }
-chia_py_streamable_macro = { version = "0.7.0", path = "../crates/chia_py_streamable_macro" }
+pyo3 = { version = "0.21.2", features = ["multiple-pymethods"] }
+chia-consensus = { version = "0.9.0", path = "../crates/chia-consensus", features = ["py-bindings"] }
+chia-bls = { version = "0.9.0", path = "../crates/chia-bls", features = ["py-bindings"]  }
+chia-protocol = { version = "0.9.0", path = "../crates/chia-protocol", features = ["py-bindings"]  }
+chia-traits = { version = "0.9.0", path = "../crates/chia-traits", features = ["py-bindings"]  }
+clvm-traits = { version = "0.9.0", path = "../crates/clvm-traits", features = ["derive", "py-bindings"] }
+clvm-utils = { version = "0.9.0", path = "../crates/clvm-utils" }
+chia_py_streamable_macro = { version = "0.9.0", path = "../crates/chia_py_streamable_macro" }
 chia_streamable_macro = { version = "0.8.0", path = "../crates/chia_streamable_macro" }
```

### Comparing `chia_rs-0.8.0/wheel/generate_type_stubs.py` & `chia_rs-0.9.0/wheel/generate_type_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,15 @@
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
 ENABLE_MESSAGE_CONDITIONS: int = ...
+DISALLOW_INFINITY_G1: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
 ENABLE_BLS_OPS: int = ...
 ENABLE_SECP_OPS: int = ...
 ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
 ENABLE_FIXED_DIV: int = ...
 ALLOW_BACKREFS: int = ...
@@ -338,15 +339,16 @@
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class BLSCache:
     def __init__(self, cache_size: Optional[int] = 50000) -> None: ...
     def len(self) -> int: ...
     def aggregate_verify(self, pks: List[G1Element], msgs: List[bytes], sig: G2Element) -> bool: ...
-    
+    def items(self) -> List[Tuple[bytes, bytes]]: ...
+    def update(self, other: List[Tuple[bytes, bytes]]) -> None: ...
 
 class AugSchemeMPL:
     @staticmethod
     def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
```

### Comparing `chia_rs-0.8.0/wheel/python/chia_rs/chia_rs.pyi` & `chia_rs-0.9.0/wheel/python/chia_rs/chia_rs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
 ENABLE_MESSAGE_CONDITIONS: int = ...
+DISALLOW_INFINITY_G1: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
 ENABLE_BLS_OPS: int = ...
 ENABLE_SECP_OPS: int = ...
 ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
 ENABLE_FIXED_DIV: int = ...
 ALLOW_BACKREFS: int = ...
@@ -81,15 +82,16 @@
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class BLSCache:
     def __init__(self, cache_size: Optional[int] = 50000) -> None: ...
     def len(self) -> int: ...
     def aggregate_verify(self, pks: List[G1Element], msgs: List[bytes], sig: G2Element) -> bool: ...
-    
+    def items(self) -> List[Tuple[bytes, bytes]]: ...
+    def update(self, other: List[Tuple[bytes, bytes]]) -> None: ...
 
 class AugSchemeMPL:
     @staticmethod
     def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
@@ -4144,14 +4146,15 @@
     MAX_BLOCK_COUNT_PER_REQUESTS: uint32
     BLOCKS_CACHE_SIZE: uint32
     MAX_GENERATOR_SIZE: uint32
     MAX_GENERATOR_REF_LIST_SIZE: uint32
     POOL_SUB_SLOT_ITERS: uint64
     SOFT_FORK2_HEIGHT: uint32
     SOFT_FORK4_HEIGHT: uint32
+    SOFT_FORK5_HEIGHT: uint32
     HARD_FORK_HEIGHT: uint32
     HARD_FORK_FIX_HEIGHT: uint32
     PLOT_FILTER_128_HEIGHT: uint32
     PLOT_FILTER_64_HEIGHT: uint32
     PLOT_FILTER_32_HEIGHT: uint32
     def __init__(
         self,
@@ -4188,14 +4191,15 @@
         MAX_BLOCK_COUNT_PER_REQUESTS: uint32,
         BLOCKS_CACHE_SIZE: uint32,
         MAX_GENERATOR_SIZE: uint32,
         MAX_GENERATOR_REF_LIST_SIZE: uint32,
         POOL_SUB_SLOT_ITERS: uint64,
         SOFT_FORK2_HEIGHT: uint32,
         SOFT_FORK4_HEIGHT: uint32,
+        SOFT_FORK5_HEIGHT: uint32,
         HARD_FORK_HEIGHT: uint32,
         HARD_FORK_FIX_HEIGHT: uint32,
         PLOT_FILTER_128_HEIGHT: uint32,
         PLOT_FILTER_64_HEIGHT: uint32,
         PLOT_FILTER_32_HEIGHT: uint32
     ) -> None: ...
     def __hash__(self) -> int: ...
@@ -4249,12 +4253,13 @@
         MAX_BLOCK_COUNT_PER_REQUESTS: Union[ uint32, _Unspec] = _Unspec(),
         BLOCKS_CACHE_SIZE: Union[ uint32, _Unspec] = _Unspec(),
         MAX_GENERATOR_SIZE: Union[ uint32, _Unspec] = _Unspec(),
         MAX_GENERATOR_REF_LIST_SIZE: Union[ uint32, _Unspec] = _Unspec(),
         POOL_SUB_SLOT_ITERS: Union[ uint64, _Unspec] = _Unspec(),
         SOFT_FORK2_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         SOFT_FORK4_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        SOFT_FORK5_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         HARD_FORK_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         HARD_FORK_FIX_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         PLOT_FILTER_128_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         PLOT_FILTER_64_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         PLOT_FILTER_32_HEIGHT: Union[ uint32, _Unspec] = _Unspec()) -> ConsensusConstants: ...
```

### Comparing `chia_rs-0.8.0/wheel/python/chia_rs/sized_byte_class.py` & `chia_rs-0.9.0/wheel/python/chia_rs/sized_byte_class.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/wheel/python/chia_rs/sized_ints.py` & `chia_rs-0.9.0/wheel/python/chia_rs/sized_ints.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/wheel/python/chia_rs/struct_stream.py` & `chia_rs-0.9.0/wheel/python/chia_rs/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/wheel/src/api.rs` & `chia_rs-0.9.0/wheel/src/api.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use crate::run_generator::{run_block_generator, run_block_generator2};
 use chia_consensus::allocator::make_allocator;
 use chia_consensus::consensus_constants::ConsensusConstants;
 use chia_consensus::gen::conditions::MempoolVisitor;
 use chia_consensus::gen::flags::{
-    AGG_SIG_ARGS, ALLOW_BACKREFS, ANALYZE_SPENDS, COND_ARGS_NIL, ENABLE_MESSAGE_CONDITIONS,
-    ENABLE_SOFTFORK_CONDITION, MEMPOOL_MODE, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS,
-    STRICT_ARGS_COUNT,
+    AGG_SIG_ARGS, ALLOW_BACKREFS, ANALYZE_SPENDS, COND_ARGS_NIL, DISALLOW_INFINITY_G1,
+    ENABLE_MESSAGE_CONDITIONS, ENABLE_SOFTFORK_CONDITION, MEMPOOL_MODE,
+    NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
 };
 use chia_consensus::gen::owned_conditions::{OwnedSpend, OwnedSpendBundleConditions};
 use chia_consensus::gen::run_puzzle::run_puzzle as native_run_puzzle;
 use chia_consensus::gen::solution_generator::solution_generator as native_solution_generator;
 use chia_consensus::gen::solution_generator::solution_generator_backrefs as native_solution_generator_backrefs;
 use chia_consensus::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
 use chia_consensus::merkle_tree::{validate_merkle_proof, MerkleSet};
@@ -40,14 +40,15 @@
     TransactionsInfo, UnfinishedBlock, UnfinishedHeaderBlock, VDFInfo, VDFProof, WeightProof,
 };
 use clvm_utils::tree_hash_from_bytes;
 use clvmr::{ENABLE_BLS_OPS_OUTSIDE_GUARD, ENABLE_FIXED_DIV, LIMIT_HEAP, NO_UNKNOWN_OPS};
 use pyo3::buffer::PyBuffer;
 use pyo3::exceptions::{PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
+use pyo3::pybacked::PyBackedBytes;
 use pyo3::types::PyBytes;
 use pyo3::types::PyList;
 use pyo3::types::PyTuple;
 use pyo3::wrap_pyfunction;
 use std::iter::zip;
 
 use crate::run_program::{run_chia_program, serialized_length};
@@ -62,28 +63,31 @@
 use clvmr::reduction::Reduction;
 use clvmr::run_program;
 use clvmr::serde::node_to_bytes;
 use clvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
 use clvmr::ChiaDialect;
 
 use chia_bls::{
-    hash_to_g2 as native_hash_to_g2, BLSCache, DerivableKey, GTElement, PublicKey, SecretKey,
+    hash_to_g2 as native_hash_to_g2, BlsCache, DerivableKey, GTElement, PublicKey, SecretKey,
     Signature,
 };
 
 #[pyfunction]
 pub fn compute_merkle_set_root<'p>(
     py: Python<'p>,
     values: Vec<&'p PyBytes>,
-) -> PyResult<&'p PyBytes> {
+) -> PyResult<Bound<'p, PyBytes>> {
     let mut buffer = Vec::<[u8; 32]>::with_capacity(values.len());
     for b in values {
         buffer.push(b.as_bytes().try_into()?);
     }
-    Ok(PyBytes::new(py, &compute_merkle_root_impl(&mut buffer)))
+    Ok(PyBytes::new_bound(
+        py,
+        &compute_merkle_root_impl(&mut buffer),
+    ))
 }
 
 #[pyfunction]
 pub fn confirm_included_already_hashed(
     root: Bytes32,
     item: Bytes32,
     proof: &[u8],
@@ -100,35 +104,35 @@
 ) -> PyResult<bool> {
     validate_merkle_proof(proof, (&item).into(), (&root).into())
         .map_err(|_| PyValueError::new_err("Invalid proof"))
         .map(|r| !r)
 }
 
 #[pyfunction]
-pub fn tree_hash(py: Python, blob: PyBuffer<u8>) -> PyResult<&PyBytes> {
+pub fn tree_hash(py: Python, blob: PyBuffer<u8>) -> PyResult<Bound<PyBytes>> {
     if !blob.is_c_contiguous() {
         panic!("tree_hash() must be called with a contiguous buffer");
     }
     let slice =
         unsafe { std::slice::from_raw_parts(blob.buf_ptr() as *const u8, blob.len_bytes()) };
-    Ok(PyBytes::new(py, &tree_hash_from_bytes(slice)?))
+    Ok(PyBytes::new_bound(py, &tree_hash_from_bytes(slice)?))
 }
 
 #[allow(clippy::too_many_arguments)]
 #[pyfunction]
 pub fn get_puzzle_and_solution_for_coin(
     py: Python<'_>,
     program: PyBuffer<u8>,
     args: PyBuffer<u8>,
     max_cost: Cost,
     find_parent: Bytes32,
     find_amount: u64,
     find_ph: Bytes32,
     flags: u32,
-) -> PyResult<(&PyBytes, &PyBytes)> {
+) -> PyResult<(Bound<PyBytes>, Bound<PyBytes>)> {
     let mut allocator = make_allocator(LIMIT_HEAP);
 
     if !program.is_c_contiguous() {
         panic!("program must be contiguous");
     }
     let program =
         unsafe { std::slice::from_raw_parts(program.buf_ptr() as *const u8, program.len_bytes()) };
@@ -164,16 +168,16 @@
         } else {
             node_to_bytes
         };
     */
     match r {
         Err(eval_err) => eval_err_to_pyresult(eval_err, allocator),
         Ok((puzzle, solution)) => Ok((
-            PyBytes::new(py, &serialize(&allocator, puzzle)?),
-            PyBytes::new(py, &serialize(&allocator, solution)?),
+            PyBytes::new_bound(py, &serialize(&allocator, puzzle)?),
+            PyBytes::new_bound(py, &serialize(&allocator, solution)?),
         )),
     }
 }
 
 #[pyfunction]
 fn run_puzzle(
     puzzle: &[u8],
@@ -188,38 +192,42 @@
         &mut a, puzzle, solution, parent_id, amount, max_cost, flags,
     )?;
     Ok(OwnedSpendBundleConditions::from(&a, conds)?)
 }
 
 // this is like a CoinSpend but with references to the puzzle and solution,
 // rather than owning them
-type CoinSpendRef<'a> = (Coin, &'a [u8], &'a [u8]);
+type CoinSpendRef = (Coin, PyBackedBytes, PyBackedBytes);
 
-fn convert_list_of_tuples(spends: &PyAny) -> PyResult<Vec<CoinSpendRef>> {
+fn convert_list_of_tuples(spends: &Bound<PyAny>) -> PyResult<Vec<CoinSpendRef>> {
     let mut native_spends = Vec::<CoinSpendRef>::new();
     for s in spends.iter()? {
-        let tuple = s?.downcast::<PyTuple>()?;
+        let s = s?;
+        let tuple = s.downcast::<PyTuple>()?;
         let coin = tuple.get_item(0)?.extract::<Coin>()?;
-        let puzzle = tuple.get_item(1)?.extract::<&[u8]>()?;
-        let solution = tuple.get_item(2)?.extract::<&[u8]>()?;
+        let puzzle = tuple.get_item(1)?.extract::<PyBackedBytes>()?;
+        let solution = tuple.get_item(2)?.extract::<PyBackedBytes>()?;
         native_spends.push((coin, puzzle, solution));
     }
     Ok(native_spends)
 }
 
 #[pyfunction]
-fn solution_generator<'p>(py: Python<'p>, spends: &PyAny) -> PyResult<&'p PyBytes> {
+fn solution_generator<'p>(py: Python<'p>, spends: &Bound<PyAny>) -> PyResult<Bound<'p, PyBytes>> {
     let spends = convert_list_of_tuples(spends)?;
-    Ok(PyBytes::new(py, &native_solution_generator(spends)?))
+    Ok(PyBytes::new_bound(py, &native_solution_generator(spends)?))
 }
 
 #[pyfunction]
-fn solution_generator_backrefs<'p>(py: Python<'p>, spends: &PyAny) -> PyResult<&'p PyBytes> {
+fn solution_generator_backrefs<'p>(
+    py: Python<'p>,
+    spends: &Bound<PyAny>,
+) -> PyResult<Bound<'p, PyBytes>> {
     let spends = convert_list_of_tuples(spends)?;
-    Ok(PyBytes::new(
+    Ok(PyBytes::new_bound(
         py,
         &native_solution_generator_backrefs(spends)?,
     ))
 }
 
 #[pyclass]
 struct AugSchemeMPL {}
@@ -236,29 +244,33 @@
                 chia_bls::sign_raw(pk, aug_msg)
             }
             None => chia_bls::sign(pk, msg),
         }
     }
 
     #[staticmethod]
-    pub fn aggregate(sigs: &PyList) -> PyResult<Signature> {
+    pub fn aggregate(sigs: &Bound<PyList>) -> PyResult<Signature> {
         let mut ret = Signature::default();
         for p2 in sigs {
             ret += &p2.extract::<Signature>()?;
         }
         Ok(ret)
     }
 
     #[staticmethod]
     pub fn verify(pk: &PublicKey, msg: &[u8], sig: &Signature) -> bool {
         chia_bls::verify(sig, pk, msg)
     }
 
     #[staticmethod]
-    pub fn aggregate_verify(pks: &PyList, msgs: &PyList, sig: &Signature) -> PyResult<bool> {
+    pub fn aggregate_verify(
+        pks: &Bound<PyList>,
+        msgs: &Bound<PyList>,
+        sig: &Signature,
+    ) -> PyResult<bool> {
         let mut data = Vec::<(PublicKey, Vec<u8>)>::new();
         if pks.len() != msgs.len() {
             return Err(PyRuntimeError::new_err(
                 "aggregate_verify expects the same number of public keys as messages",
             ));
         }
         for (pk, msg) in zip(pks, msgs) {
@@ -336,28 +348,28 @@
 
 #[pyfunction]
 fn fast_forward_singleton<'p>(
     py: Python<'p>,
     spend: &CoinSpend,
     new_coin: &Coin,
     new_parent: &Coin,
-) -> PyResult<&'p PyBytes> {
+) -> PyResult<Bound<'p, PyBytes>> {
     let mut a = make_allocator(LIMIT_HEAP);
     let puzzle = node_from_bytes(&mut a, spend.puzzle_reveal.as_slice())?;
     let solution = node_from_bytes(&mut a, spend.solution.as_slice())?;
 
     let new_solution = native_ff(&mut a, puzzle, solution, &spend.coin, new_coin, new_parent)?;
-    Ok(PyBytes::new(
+    Ok(PyBytes::new_bound(
         py,
         node_to_bytes(&a, new_solution)?.as_slice(),
     ))
 }
 
 #[pymodule]
-pub fn chia_rs(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn chia_rs(_py: Python, m: &Bound<PyModule>) -> PyResult<()> {
     // generator functions
     m.add_function(wrap_pyfunction!(run_block_generator, m)?)?;
     m.add_function(wrap_pyfunction!(run_block_generator2, m)?)?;
     m.add_function(wrap_pyfunction!(run_puzzle, m)?)?;
     m.add_function(wrap_pyfunction!(solution_generator, m)?)?;
     m.add_function(wrap_pyfunction!(solution_generator_backrefs, m)?)?;
     m.add_function(wrap_pyfunction!(supports_fast_forward, m)?)?;
@@ -392,14 +404,15 @@
     m.add(
         "NO_RELATIVE_CONDITIONS_ON_EPHEMERAL",
         NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
     )?;
     m.add("MEMPOOL_MODE", MEMPOOL_MODE)?;
     m.add("ALLOW_BACKREFS", ALLOW_BACKREFS)?;
     m.add("ANALYZE_SPENDS", ANALYZE_SPENDS)?;
+    m.add("DISALLOW_INFINITY_G1", DISALLOW_INFINITY_G1)?;
 
     // Chia classes
     m.add_class::<Coin>()?;
     m.add_class::<PoolTarget>()?;
     m.add_class::<ClassgroupElement>()?;
     m.add_class::<EndOfSubSlotBundle>()?;
     m.add_class::<TransactionsInfo>()?;
@@ -525,11 +538,11 @@
     // facilities from chia-bls
 
     m.add_class::<PublicKey>()?;
     m.add_class::<Signature>()?;
     m.add_class::<GTElement>()?;
     m.add_class::<SecretKey>()?;
     m.add_class::<AugSchemeMPL>()?;
-    m.add_class::<BLSCache>()?;
+    m.add_class::<BlsCache>()?;
 
     Ok(())
 }
```

### Comparing `chia_rs-0.8.0/wheel/src/run_generator.rs` & `chia_rs-0.9.0/wheel/src/run_generator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 
 #[pyfunction]
 pub fn run_block_generator(
     _py: Python,
     program: PyBuffer<u8>,
-    block_refs: &PyList,
+    block_refs: &Bound<PyList>,
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Option<u32>, Option<OwnedSpendBundleConditions>)> {
     let mut allocator = make_allocator(flags);
 
     let mut refs = Vec::<&[u8]>::new();
     for g in block_refs {
@@ -64,15 +64,15 @@
     )
 }
 
 #[pyfunction]
 pub fn run_block_generator2(
     _py: Python,
     program: PyBuffer<u8>,
-    block_refs: &PyList,
+    block_refs: &Bound<PyList>,
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Option<u32>, Option<OwnedSpendBundleConditions>)> {
     let mut allocator = make_allocator(flags);
 
     let mut refs = Vec::<&[u8]>::new();
     for g in block_refs {
```

### Comparing `chia_rs-0.8.0/wheel/src/run_program.rs` & `chia_rs-0.9.0/wheel/src/run_program.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/Cargo.lock` & `chia_rs-0.9.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -272,23 +272,23 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chia"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "chia-client",
  "chia-consensus",
  "chia-protocol",
  "chia-puzzles",
  "chia-ssl",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "clvm-traits",
  "clvm-utils",
 ]
 
 [[package]]
 name = "chia-bls"
 version = "0.4.0"
@@ -304,20 +304,20 @@
  "sha2",
  "thiserror",
  "tiny-bip39",
 ]
 
 [[package]]
 name = "chia-bls"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "anyhow",
  "arbitrary",
  "blst",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "chia_py_streamable_macro",
  "criterion",
  "hex",
  "hkdf",
  "lru",
  "pyo3",
  "rand",
@@ -325,42 +325,42 @@
  "sha2",
  "thiserror",
  "tiny-bip39",
 ]
 
 [[package]]
 name = "chia-bls-fuzz"
-version = "0.0.0"
+version = "0.9.0"
 dependencies = [
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "libfuzzer-sys",
  "pyo3",
 ]
 
 [[package]]
 name = "chia-client"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "chia-protocol",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "futures-util",
  "thiserror",
  "tokio",
  "tokio-tungstenite",
  "tungstenite",
 ]
 
 [[package]]
 name = "chia-consensus"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "chia-protocol",
  "chia-puzzles",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "chia_py_streamable_macro",
  "chia_streamable_macro 0.8.0",
  "clvm-derive",
  "clvm-traits",
  "clvm-utils",
  "clvmr",
  "criterion",
@@ -377,29 +377,29 @@
 
 [[package]]
 name = "chia-fuzz"
 version = "0.6.0"
 dependencies = [
  "chia-consensus",
  "chia-protocol",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "clvm-traits",
  "clvm-utils",
  "clvmr",
  "hex-literal",
  "libfuzzer-sys",
 ]
 
 [[package]]
 name = "chia-protocol"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "arbitrary",
- "chia-bls 0.8.0",
- "chia-traits 0.8.0",
+ "chia-bls 0.9.0",
+ "chia-traits 0.9.0",
  "chia_py_streamable_macro",
  "chia_streamable_macro 0.8.0",
  "clvm-traits",
  "clvm-utils",
  "clvmr",
  "hex",
  "pyo3",
@@ -409,41 +409,41 @@
 
 [[package]]
 name = "chia-protocol-fuzz"
 version = "0.8.0"
 dependencies = [
  "arbitrary",
  "chia-protocol",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "clvm-traits",
  "clvmr",
  "hex",
  "libfuzzer-sys",
  "sha2",
 ]
 
 [[package]]
 name = "chia-puzzles"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "arbitrary",
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "chia-protocol",
  "clvm-traits",
  "clvm-utils",
  "clvmr",
  "hex",
  "hex-literal",
  "num-bigint",
  "sha2",
 ]
 
 [[package]]
 name = "chia-puzzles-fuzz"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "chia-puzzles",
  "clvm-traits",
  "clvmr",
  "libfuzzer-sys",
  "pyo3",
 ]
@@ -458,22 +458,22 @@
  "rsa",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "chia-tools"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "blocking-threadpool",
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "chia-consensus",
  "chia-protocol",
  "chia-puzzles",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "clap",
  "clvm-traits",
  "clvm-utils",
  "clvmr",
  "hex",
  "hex-literal",
  "rusqlite",
@@ -490,40 +490,40 @@
  "hex",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
 name = "chia-traits"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "chia_streamable_macro 0.8.0",
  "pyo3",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
 name = "chia_py_streamable_macro"
-version = "0.7.0"
+version = "0.9.0"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "chia_rs"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "chia-consensus",
  "chia-protocol",
- "chia-traits 0.8.0",
+ "chia-traits 0.9.0",
  "chia_py_streamable_macro",
  "chia_streamable_macro 0.8.0",
  "clvm-traits",
  "clvm-utils",
  "clvmr",
  "hex",
  "pyo3",
@@ -550,15 +550,15 @@
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "chia_wasm"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "ciborium"
 version = "0.2.2"
@@ -610,52 +610,52 @@
 
 [[package]]
 name = "clap_derive"
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
- "heck",
+ "heck 0.5.0",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "clvm-derive"
-version = "0.6.0"
+version = "0.9.0"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "clvm-traits"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
- "chia-bls 0.8.0",
+ "chia-bls 0.9.0",
  "clvm-derive",
  "clvmr",
  "hex",
  "hex-literal",
  "num-bigint",
  "pyo3",
  "thiserror",
 ]
 
 [[package]]
 name = "clvm-utils"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "clvm-traits",
  "clvmr",
  "hex",
  "rstest 0.16.0",
 ]
 
@@ -1139,14 +1139,20 @@
 checksum = "e8094feaf31ff591f651a2664fb9cfd92bba7a60ce3197265e9482ebe753c8f7"
 dependencies = [
  "hashbrown",
 ]
 
 [[package]]
 name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
+name = "heck"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "hermit-abi"
 version = "0.3.9"
@@ -1218,17 +1224,17 @@
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inventory"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
@@ -1656,14 +1662,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "ppv-lite86"
@@ -1697,72 +1709,75 @@
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
  "num-bigint",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck 0.4.1",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -2433,17 +2448,17 @@
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
@@ -2496,65 +2511,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
```

### Comparing `chia_rs-0.8.0/Cargo.toml` & `chia_rs-0.9.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["wheel"]
 
 [package]
 name = "chia"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "A meta-crate that exports all of the Chia crates in the workspace."
 authors = [
     "Richard Kiss <him@richardkiss.com>",
     "Arvid Norberg <arvid@chia.net>",
     "Brandon Haggstrom <b.haggstrom@chia.net>"
@@ -35,23 +35,23 @@
 ssl = ["dep:chia-ssl"]
 traits = ["dep:chia-traits"]
 puzzles = ["dep:chia-puzzles"]
 clvm-traits = ["dep:clvm-traits"]
 clvm-utils = ["dep:clvm-utils"]
 
 [dependencies]
-chia-bls = { path = "./crates/chia-bls", version = "0.8.0", optional = true }
-chia-client = { path = "./crates/chia-client", version = "0.8.0", optional = true }
-chia-consensus = { path = "./crates/chia-consensus", version = "0.8.0", optional = true }
-chia-protocol = { path = "./crates/chia-protocol", version = "0.8.0", optional = true }
+chia-bls = { path = "./crates/chia-bls", version = "0.9.0", optional = true }
+chia-client = { path = "./crates/chia-client", version = "0.9.0", optional = true }
+chia-consensus = { path = "./crates/chia-consensus", version = "0.9.0", optional = true }
+chia-protocol = { path = "./crates/chia-protocol", version = "0.9.0", optional = true }
 chia-ssl = { path = "./crates/chia-ssl", version = "0.7.0", optional = true }
-chia-traits = { path = "./crates/chia-traits", version = "0.8.0", optional = true }
-chia-puzzles = { path = "./crates/chia-puzzles", version = "0.8.0", optional = true }
-clvm-traits = { path = "./crates/clvm-traits", version = "0.8.0", optional = true }
-clvm-utils = { path = "./crates/clvm-utils", version = "0.8.0", optional = true }
+chia-traits = { path = "./crates/chia-traits", version = "0.9.0", optional = true }
+chia-puzzles = { path = "./crates/chia-puzzles", version = "0.9.0", optional = true }
+clvm-traits = { path = "./crates/clvm-traits", version = "0.9.0", optional = true }
+clvm-utils = { path = "./crates/clvm-utils", version = "0.9.0", optional = true }
 
 [profile.release]
 lto = "thin"
 
 # This is also necessary in `wheel/Cargo.toml` to make sure the `wheel` crate builds as well.
 # Pin the `blst` dependency to the correct revision, since the fix has not been properly released yet.
 [patch.crates-io]
```

### Comparing `chia_rs-0.8.0/python/chia_rs/chia_rs.pyi` & `chia_rs-0.9.0/python/chia_rs/chia_rs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
 ENABLE_MESSAGE_CONDITIONS: int = ...
+DISALLOW_INFINITY_G1: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
 ENABLE_BLS_OPS: int = ...
 ENABLE_SECP_OPS: int = ...
 ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
 ENABLE_FIXED_DIV: int = ...
 ALLOW_BACKREFS: int = ...
@@ -81,15 +82,16 @@
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class BLSCache:
     def __init__(self, cache_size: Optional[int] = 50000) -> None: ...
     def len(self) -> int: ...
     def aggregate_verify(self, pks: List[G1Element], msgs: List[bytes], sig: G2Element) -> bool: ...
-    
+    def items(self) -> List[Tuple[bytes, bytes]]: ...
+    def update(self, other: List[Tuple[bytes, bytes]]) -> None: ...
 
 class AugSchemeMPL:
     @staticmethod
     def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
@@ -4144,14 +4146,15 @@
     MAX_BLOCK_COUNT_PER_REQUESTS: uint32
     BLOCKS_CACHE_SIZE: uint32
     MAX_GENERATOR_SIZE: uint32
     MAX_GENERATOR_REF_LIST_SIZE: uint32
     POOL_SUB_SLOT_ITERS: uint64
     SOFT_FORK2_HEIGHT: uint32
     SOFT_FORK4_HEIGHT: uint32
+    SOFT_FORK5_HEIGHT: uint32
     HARD_FORK_HEIGHT: uint32
     HARD_FORK_FIX_HEIGHT: uint32
     PLOT_FILTER_128_HEIGHT: uint32
     PLOT_FILTER_64_HEIGHT: uint32
     PLOT_FILTER_32_HEIGHT: uint32
     def __init__(
         self,
@@ -4188,14 +4191,15 @@
         MAX_BLOCK_COUNT_PER_REQUESTS: uint32,
         BLOCKS_CACHE_SIZE: uint32,
         MAX_GENERATOR_SIZE: uint32,
         MAX_GENERATOR_REF_LIST_SIZE: uint32,
         POOL_SUB_SLOT_ITERS: uint64,
         SOFT_FORK2_HEIGHT: uint32,
         SOFT_FORK4_HEIGHT: uint32,
+        SOFT_FORK5_HEIGHT: uint32,
         HARD_FORK_HEIGHT: uint32,
         HARD_FORK_FIX_HEIGHT: uint32,
         PLOT_FILTER_128_HEIGHT: uint32,
         PLOT_FILTER_64_HEIGHT: uint32,
         PLOT_FILTER_32_HEIGHT: uint32
     ) -> None: ...
     def __hash__(self) -> int: ...
@@ -4249,12 +4253,13 @@
         MAX_BLOCK_COUNT_PER_REQUESTS: Union[ uint32, _Unspec] = _Unspec(),
         BLOCKS_CACHE_SIZE: Union[ uint32, _Unspec] = _Unspec(),
         MAX_GENERATOR_SIZE: Union[ uint32, _Unspec] = _Unspec(),
         MAX_GENERATOR_REF_LIST_SIZE: Union[ uint32, _Unspec] = _Unspec(),
         POOL_SUB_SLOT_ITERS: Union[ uint64, _Unspec] = _Unspec(),
         SOFT_FORK2_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         SOFT_FORK4_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        SOFT_FORK5_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         HARD_FORK_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         HARD_FORK_FIX_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         PLOT_FILTER_128_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         PLOT_FILTER_64_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
         PLOT_FILTER_32_HEIGHT: Union[ uint32, _Unspec] = _Unspec()) -> ConsensusConstants: ...
```

### Comparing `chia_rs-0.8.0/python/chia_rs/struct_stream.py` & `chia_rs-0.9.0/python/chia_rs/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/python/chia_rs/sized_ints.py` & `chia_rs-0.9.0/python/chia_rs/sized_ints.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.8.0/python/chia_rs/sized_byte_class.py` & `chia_rs-0.9.0/python/chia_rs/sized_byte_class.py`

 * *Files identical despite different names*

