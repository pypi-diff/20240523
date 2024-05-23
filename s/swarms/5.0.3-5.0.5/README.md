# Comparing `tmp/swarms-5.0.3.tar.gz` & `tmp/swarms-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-5.0.3.tar", max compression
+gzip compressed data, was "swarms-5.0.5.tar", max compression
```

## Comparing `swarms-5.0.3.tar` & `swarms-5.0.5.tar`

### file list

```diff
@@ -1,217 +1,207 @@
--rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-5.0.3/LICENSE
--rw-r--r--   0        0        0    37907 2024-05-17 04:37:25.650827 swarms-5.0.3/README.md
--rw-r--r--   0        0        0     1790 2024-05-19 03:24:03.190053 swarms-5.0.3/pyproject.toml
--rw-r--r--   0        0        0      590 2024-05-10 15:36:40.566920 swarms-5.0.3/swarms/__init__.py
--rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-5.0.3/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-5.0.3/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-5.0.3/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-5.0.3/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-5.0.3/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3491 2024-04-27 21:17:36.621105 swarms-5.0.3/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-5.0.3/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4940 2024-04-27 21:17:36.621832 swarms-5.0.3/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5504 2024-05-08 21:09:56.813124 swarms-5.0.3/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-5.0.3/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-5.0.3/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-5.0.3/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      613 2024-04-27 21:17:36.623130 swarms-5.0.3/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-5.0.3/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-5.0.3/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2823 2024-04-27 21:17:36.624819 swarms-5.0.3/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-5.0.3/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-5.0.3/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-5.0.3/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-5.0.3/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     2533 2024-05-18 23:20:02.171975 swarms-5.0.3/swarms/models/__init__.py
--rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-5.0.3/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13168 2024-04-27 21:17:36.635065 swarms-5.0.3/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-5.0.3/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2475 2024-04-27 21:17:36.635700 swarms-5.0.3/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3163 2024-04-27 21:17:36.636332 swarms-5.0.3/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-5.0.3/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-5.0.3/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-5.0.3/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-5.0.3/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     2726 2024-04-27 21:17:36.637208 swarms-5.0.3/swarms/models/fire_function.py
--rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-5.0.3/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-5.0.3/swarms/models/gemini.py
--rw-r--r--   0        0        0    14236 2024-05-14 15:55:46.753852 swarms-5.0.3/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    12996 2024-04-27 21:17:36.638023 swarms-5.0.3/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1826 2024-04-27 21:17:36.638977 swarms-5.0.3/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-5.0.3/swarms/models/idefics.py
--rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-5.0.3/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-5.0.3/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     2529 2024-05-18 17:55:07.794536 swarms-5.0.3/swarms/models/llama3_hosted.py
--rw-r--r--   0        0        0     6581 2024-04-27 21:17:36.639950 swarms-5.0.3/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-5.0.3/swarms/models/llava.py
--rw-r--r--   0        0        0     4286 2024-04-27 21:17:36.641073 swarms-5.0.3/swarms/models/mistral.py
--rw-r--r--   0        0        0     2147 2024-04-27 21:17:36.642823 swarms-5.0.3/swarms/models/mixtral.py
--rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-5.0.3/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     2881 2024-05-18 16:58:15.348268 swarms-5.0.3/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-5.0.3/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2464 2024-04-27 21:17:36.644597 swarms-5.0.3/swarms/models/open_router.py
--rw-r--r--   0        0        0      106 2024-04-25 14:24:46.757474 swarms-5.0.3/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3167 2024-04-27 21:17:36.645494 swarms-5.0.3/swarms/models/openai_tts.py
--rw-r--r--   0        0        0       93 2024-04-25 14:24:46.757393 swarms-5.0.3/swarms/models/palm.py
--rw-r--r--   0        0        0     2160 2024-05-08 21:09:56.821210 swarms-5.0.3/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-5.0.3/swarms/models/qwen.py
--rw-r--r--   0        0        0     3561 2024-05-18 05:48:32.478953 swarms-5.0.3/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-5.0.3/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-5.0.3/swarms/models/speecht5.py
--rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-5.0.3/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     3948 2024-04-27 21:17:36.646243 swarms-5.0.3/swarms/models/together.py
--rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-5.0.3/swarms/models/types.py
--rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-5.0.3/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-5.0.3/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     3666 2024-05-18 16:58:15.352844 swarms-5.0.3/swarms/models/zeroscope.py
--rw-r--r--   0        0        0        0 2024-05-01 03:43:07.020028 swarms-5.0.3/swarms/prebuilt_swarms/__init__.py
--rw-r--r--   0        0        0      692 2024-05-08 21:09:56.824718 swarms-5.0.3/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-5.0.3/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-5.0.3/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-5.0.3/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-5.0.3/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-5.0.3/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7113 2024-05-08 21:09:56.832506 swarms-5.0.3/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-5.0.3/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0     1148 2024-05-01 03:43:07.021040 swarms-5.0.3/swarms/prompts/aot_prompt.py
--rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-5.0.3/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-5.0.3/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-5.0.3/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-5.0.3/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-5.0.3/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-5.0.3/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-5.0.3/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7152 2024-05-18 17:23:48.186668 swarms-5.0.3/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-5.0.3/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-5.0.3/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-5.0.3/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-5.0.3/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-5.0.3/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-5.0.3/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-5.0.3/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-5.0.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-5.0.3/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-5.0.3/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-5.0.3/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-5.0.3/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-5.0.3/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-5.0.3/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-5.0.3/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-5.0.3/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-5.0.3/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-5.0.3/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-5.0.3/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-5.0.3/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-5.0.3/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-5.0.3/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-5.0.3/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-5.0.3/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-5.0.3/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-5.0.3/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-5.0.3/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-5.0.3/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-5.0.3/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-5.0.3/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-5.0.3/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     5554 2024-05-19 03:25:09.324726 swarms-5.0.3/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-5.0.3/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0     4152 2024-05-19 03:30:07.885255 swarms-5.0.3/swarms/structs/__init__.py
--rw-r--r--   0        0        0    60110 2024-05-16 20:36:45.500176 swarms-5.0.3/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-5.0.3/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-5.0.3/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-5.0.3/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-5.0.3/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12437 2024-04-23 01:08:13.052177 swarms-5.0.3/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    19446 2024-05-08 21:09:56.884181 swarms-5.0.3/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12161 2024-05-08 21:09:56.888358 swarms-5.0.3/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-5.0.3/swarms/structs/block_wrapper.py
--rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-5.0.3/swarms/structs/blocks_dict.py
--rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-5.0.3/swarms/structs/blocks_list.py
--rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-5.0.3/swarms/structs/company.py
--rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-5.0.3/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14685 2024-04-26 04:55:42.709791 swarms-5.0.3/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-5.0.3/swarms/structs/debate.py
--rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-5.0.3/swarms/structs/document.py
--rw-r--r--   0        0        0     4775 2024-04-26 04:55:42.710484 swarms-5.0.3/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     3699 2024-05-19 03:27:26.615693 swarms-5.0.3/swarms/structs/hiearchical_swarm.py
--rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-5.0.3/swarms/structs/long_swarm.py
--rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-5.0.3/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-5.0.3/swarms/structs/message.py
--rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-5.0.3/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      855 2024-04-27 21:17:36.650763 swarms-5.0.3/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-5.0.3/swarms/structs/model_parallizer.py
--rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-5.0.3/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-5.0.3/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-5.0.3/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0      371 2024-05-16 00:24:04.336048 swarms-5.0.3/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0      182 2024-04-28 21:24:54.081857 swarms-5.0.3/swarms/structs/plan.py
--rw-r--r--   0        0        0    11353 2024-05-16 01:32:38.721849 swarms-5.0.3/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-5.0.3/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     3256 2024-05-13 20:15:02.129223 swarms-5.0.3/swarms/structs/round_robin.py
--rw-r--r--   0        0        0     6764 2024-04-23 01:17:51.964275 swarms-5.0.3/swarms/structs/schemas.py
--rw-r--r--   0        0        0     2956 2024-05-08 21:09:56.891925 swarms-5.0.3/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-5.0.3/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0      709 2024-05-08 21:09:56.895373 swarms-5.0.3/swarms/structs/step.py
--rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-5.0.3/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-5.0.3/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-5.0.3/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-5.0.3/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-5.0.3/swarms/structs/utils.py
--rw-r--r--   0        0        0     7403 2024-04-24 00:20:16.136940 swarms-5.0.3/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-5.0.3/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-5.0.3/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-5.0.3/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-5.0.3/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-5.0.3/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-5.0.3/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2675 2024-04-23 23:56:19.053195 swarms-5.0.3/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1879 2024-04-24 21:57:07.051275 swarms-5.0.3/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1680 2024-05-08 21:09:56.899526 swarms-5.0.3/swarms/tools/__init__.py
--rw-r--r--   0        0        0    12525 2024-05-08 21:09:56.906505 swarms-5.0.3/swarms/tools/base_tool.py
--rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-5.0.3/swarms/tools/code_interpreter.py
--rw-r--r--   0        0        0     5367 2024-05-08 21:09:56.913861 swarms-5.0.3/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-5.0.3/swarms/tools/function_util.py
--rw-r--r--   0        0        0    14241 2024-04-27 21:17:36.654062 swarms-5.0.3/swarms/tools/json_former.py
--rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-5.0.3/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-5.0.3/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-5.0.3/swarms/tools/math_eval.py
--rw-r--r--   0        0        0      978 2024-04-23 23:18:25.950155 swarms-5.0.3/swarms/tools/openai_func_calling_schema.py
--rw-r--r--   0        0        0    13875 2024-05-08 21:09:56.921184 swarms-5.0.3/swarms/tools/openai_tool_creator_decorator.py
--rw-r--r--   0        0        0    15564 2024-04-27 21:17:36.657668 swarms-5.0.3/swarms/tools/py_func_to_openai_func_str.py
--rw-r--r--   0        0        0     4275 2024-05-08 21:09:56.925611 swarms-5.0.3/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-5.0.3/swarms/tools/tool.py
--rw-r--r--   0        0        0     6170 2024-05-08 21:09:56.930060 swarms-5.0.3/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-5.0.3/swarms/utils/README.md
--rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-5.0.3/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-5.0.3/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-5.0.3/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-5.0.3/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-5.0.3/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-5.0.3/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-5.0.3/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-5.0.3/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-5.0.3/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-5.0.3/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-5.0.3/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-5.0.3/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-5.0.3/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-5.0.3/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-5.0.3/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-5.0.3/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     4232 2024-05-17 00:01:56.878497 swarms-5.0.3/swarms/utils/get_total_gpus.py
--rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-5.0.3/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-5.0.3/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-5.0.3/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-5.0.3/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-5.0.3/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-5.0.3/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-5.0.3/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-5.0.3/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-5.0.3/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-5.0.3/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-5.0.3/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-5.0.3/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1315 2024-04-25 14:49:22.838126 swarms-5.0.3/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-5.0.3/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    40527 1970-01-01 00:00:00.000000 swarms-5.0.3/setup.py
--rw-r--r--   0        0        0    39413 1970-01-01 00:00:00.000000 swarms-5.0.3/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-05-20 23:12:19.525914 swarms-5.0.5/LICENSE
+-rw-r--r--   0        0        0    33713 2024-05-21 21:17:55.232096 swarms-5.0.5/README.md
+-rw-r--r--   0        0        0     1790 2024-05-21 05:06:14.076867 swarms-5.0.5/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-05-20 23:12:19.584595 swarms-5.0.5/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-20 23:12:19.584679 swarms-5.0.5/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-05-20 23:12:19.584738 swarms-5.0.5/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-05-20 23:12:19.584796 swarms-5.0.5/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-05-20 23:12:19.584880 swarms-5.0.5/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-05-20 23:12:19.584947 swarms-5.0.5/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-05-20 23:12:19.585001 swarms-5.0.5/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-05-20 23:12:19.585048 swarms-5.0.5/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-05-20 23:12:19.585129 swarms-5.0.5/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5504 2024-05-20 23:12:19.585192 swarms-5.0.5/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-05-20 23:12:19.585283 swarms-5.0.5/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-20 23:12:19.585343 swarms-5.0.5/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-05-20 23:12:19.585425 swarms-5.0.5/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      613 2024-05-20 23:12:19.585515 swarms-5.0.5/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-20 23:12:19.585565 swarms-5.0.5/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-05-20 23:12:19.585621 swarms-5.0.5/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-05-20 23:12:19.585702 swarms-5.0.5/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-05-20 23:12:19.585767 swarms-5.0.5/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-05-20 23:12:19.585826 swarms-5.0.5/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-05-20 23:12:19.585895 swarms-5.0.5/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-05-20 23:12:19.585978 swarms-5.0.5/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2392 2024-05-21 05:06:54.045652 swarms-5.0.5/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2052 2024-05-21 00:48:59.027928 swarms-5.0.5/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-05-20 23:12:19.586207 swarms-5.0.5/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-05-20 23:12:19.586302 swarms-5.0.5/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-05-20 23:12:19.586361 swarms-5.0.5/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-05-20 23:12:19.586416 swarms-5.0.5/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-05-20 23:12:19.586490 swarms-5.0.5/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-05-20 23:12:19.586608 swarms-5.0.5/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-05-20 23:12:19.586690 swarms-5.0.5/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-05-20 23:12:19.586747 swarms-5.0.5/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     3022 2024-05-20 23:12:19.586804 swarms-5.0.5/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-05-20 23:12:19.586891 swarms-5.0.5/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14236 2024-05-20 23:12:19.586973 swarms-5.0.5/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-05-20 23:12:19.587047 swarms-5.0.5/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-05-20 23:12:19.587108 swarms-5.0.5/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-05-20 23:12:19.587202 swarms-5.0.5/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-05-20 23:12:19.587276 swarms-5.0.5/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-05-20 23:12:19.587347 swarms-5.0.5/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     2599 2024-05-21 05:06:21.835242 swarms-5.0.5/swarms/models/llama3_hosted.py
+-rw-r--r--   0        0        0     6581 2024-05-20 23:12:19.587506 swarms-5.0.5/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-05-20 23:12:19.587573 swarms-5.0.5/swarms/models/llava.py
+-rw-r--r--   0        0        0     2056 2024-05-20 23:12:19.587792 swarms-5.0.5/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     2881 2024-05-20 23:12:19.587858 swarms-5.0.5/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-05-20 23:12:19.587917 swarms-5.0.5/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-05-20 23:12:19.587972 swarms-5.0.5/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-05-20 23:12:19.588047 swarms-5.0.5/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-05-20 23:12:19.588099 swarms-5.0.5/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-05-20 23:12:19.588149 swarms-5.0.5/swarms/models/palm.py
+-rw-r--r--   0        0        0     2160 2024-05-20 23:12:19.588204 swarms-5.0.5/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-05-20 23:12:19.588296 swarms-5.0.5/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3561 2024-05-20 23:12:19.588355 swarms-5.0.5/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-05-20 23:12:19.588421 swarms-5.0.5/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     8244 2024-05-20 23:12:19.588474 swarms-5.0.5/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     3948 2024-05-20 23:12:19.588553 swarms-5.0.5/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-05-20 23:12:19.588607 swarms-5.0.5/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-05-20 23:12:19.588664 swarms-5.0.5/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-05-20 23:12:19.588711 swarms-5.0.5/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3666 2024-05-20 23:12:19.588784 swarms-5.0.5/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.588836 swarms-5.0.5/swarms/prebuilt_swarms/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-20 23:12:19.588923 swarms-5.0.5/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-05-20 23:12:19.588988 swarms-5.0.5/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-05-20 23:12:19.589069 swarms-5.0.5/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-05-20 23:12:19.589128 swarms-5.0.5/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-05-20 23:12:19.589180 swarms-5.0.5/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-05-20 23:12:19.589236 swarms-5.0.5/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7113 2024-05-20 23:12:19.589316 swarms-5.0.5/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-05-20 23:12:19.589377 swarms-5.0.5/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-05-20 23:12:19.589426 swarms-5.0.5/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-05-20 23:12:19.589498 swarms-5.0.5/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-05-20 23:12:19.589584 swarms-5.0.5/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-05-20 23:12:19.589647 swarms-5.0.5/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-05-20 23:12:19.589703 swarms-5.0.5/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-05-20 23:12:19.589756 swarms-5.0.5/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-05-20 23:12:19.589834 swarms-5.0.5/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-05-20 23:12:19.589885 swarms-5.0.5/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7152 2024-05-20 23:12:19.589946 swarms-5.0.5/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-05-20 23:12:19.590009 swarms-5.0.5/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-05-20 23:12:19.590089 swarms-5.0.5/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-05-20 23:12:19.590152 swarms-5.0.5/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-05-20 23:12:19.590207 swarms-5.0.5/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-05-20 23:12:19.590267 swarms-5.0.5/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-05-20 23:12:19.590358 swarms-5.0.5/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-05-20 23:12:19.590418 swarms-5.0.5/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-05-20 23:12:19.590489 swarms-5.0.5/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.590550 swarms-5.0.5/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-05-20 23:12:19.590626 swarms-5.0.5/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-05-20 23:12:19.590685 swarms-5.0.5/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0     2149 2024-05-20 23:12:19.590738 swarms-5.0.5/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-05-20 23:12:19.590803 swarms-5.0.5/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-05-20 23:12:19.590895 swarms-5.0.5/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-05-20 23:12:19.590958 swarms-5.0.5/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-05-20 23:12:19.591020 swarms-5.0.5/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-05-20 23:12:19.591076 swarms-5.0.5/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-05-20 23:12:19.591117 swarms-5.0.5/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-05-20 23:12:19.591208 swarms-5.0.5/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-05-20 23:12:19.591263 swarms-5.0.5/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     2679 2024-05-20 23:12:19.591326 swarms-5.0.5/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-05-20 23:12:19.591419 swarms-5.0.5/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-05-20 23:12:19.591487 swarms-5.0.5/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-05-20 23:12:19.591551 swarms-5.0.5/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-05-20 23:12:19.591612 swarms-5.0.5/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-05-20 23:12:19.591714 swarms-5.0.5/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-05-20 23:12:19.591774 swarms-5.0.5/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-05-20 23:12:19.591847 swarms-5.0.5/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     4288 2024-05-20 23:12:19.591952 swarms-5.0.5/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-05-20 23:12:19.592013 swarms-5.0.5/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-05-20 23:12:19.592103 swarms-5.0.5/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     5554 2024-05-20 23:12:19.592180 swarms-5.0.5/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-05-20 23:12:19.592230 swarms-5.0.5/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-21 03:27:54.652576 swarms-5.0.5/swarms/schemas/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-21 05:06:25.218133 swarms-5.0.5/swarms/schemas/plan.py
+-rw-r--r--   0        0        0     6764 2024-05-20 23:12:19.594641 swarms-5.0.5/swarms/schemas/schemas.py
+-rw-r--r--   0        0        0      709 2024-05-20 23:12:19.594792 swarms-5.0.5/swarms/schemas/step.py
+-rw-r--r--   0        0        0     4005 2024-05-21 05:06:15.133196 swarms-5.0.5/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    60111 2024-05-21 05:06:23.482699 swarms-5.0.5/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-05-20 23:12:19.592548 swarms-5.0.5/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-05-20 23:12:19.592611 swarms-5.0.5/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3777 2024-05-20 23:12:19.592668 swarms-5.0.5/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     6624 2024-05-20 23:12:19.592755 swarms-5.0.5/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-05-20 23:12:19.592817 swarms-5.0.5/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    19446 2024-05-20 23:12:19.592905 swarms-5.0.5/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12161 2024-05-20 23:12:19.593000 swarms-5.0.5/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     5265 2024-05-21 00:48:59.119899 swarms-5.0.5/swarms/structs/company.py
+-rw-r--r--   0        0        0     4738 2024-05-21 03:30:50.037223 swarms-5.0.5/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-05-20 23:12:19.593392 swarms-5.0.5/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12608 2024-05-20 23:12:19.593456 swarms-5.0.5/swarms/structs/debate.py
+-rw-r--r--   0        0        0     4834 2024-05-20 23:12:19.593607 swarms-5.0.5/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     3684 2024-05-21 05:06:56.355513 swarms-5.0.5/swarms/structs/hiearchical_swarm.py
+-rw-r--r--   0        0        0     7012 2024-05-20 23:12:19.593787 swarms-5.0.5/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      621 2024-05-21 05:06:56.355487 swarms-5.0.5/swarms/structs/message.py
+-rw-r--r--   0        0        0     7397 2024-05-20 23:12:19.593913 swarms-5.0.5/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-05-20 23:12:19.593973 swarms-5.0.5/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     8390 2024-05-20 23:12:19.594122 swarms-5.0.5/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-05-20 23:12:19.594191 swarms-5.0.5/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-05-20 23:12:19.594250 swarms-5.0.5/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-05-20 23:12:19.594301 swarms-5.0.5/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0     9900 2024-05-21 03:26:12.085452 swarms-5.0.5/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     3011 2024-05-20 23:12:19.594499 swarms-5.0.5/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     3256 2024-05-20 23:12:19.594554 swarms-5.0.5/swarms/structs/round_robin.py
+-rw-r--r--   0        0        0     2956 2024-05-20 23:12:19.594695 swarms-5.0.5/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2442 2024-05-20 23:12:19.594743 swarms-5.0.5/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0    10684 2024-05-20 23:12:19.594876 swarms-5.0.5/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-05-20 23:12:19.594944 swarms-5.0.5/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8251 2024-05-20 23:12:19.595011 swarms-5.0.5/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-05-20 23:12:19.595073 swarms-5.0.5/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3511 2024-05-20 23:12:19.595145 swarms-5.0.5/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-05-20 23:12:19.595210 swarms-5.0.5/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-05-20 23:12:19.595297 swarms-5.0.5/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-05-20 23:12:19.595348 swarms-5.0.5/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-05-20 23:12:19.595426 swarms-5.0.5/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-05-20 23:12:19.595476 swarms-5.0.5/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-05-20 23:12:19.595528 swarms-5.0.5/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-05-20 23:12:19.595576 swarms-5.0.5/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-05-20 23:12:19.595649 swarms-5.0.5/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-05-20 23:12:19.595698 swarms-5.0.5/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1680 2024-05-20 23:12:19.595775 swarms-5.0.5/swarms/tools/__init__.py
+-rw-r--r--   0        0        0    12610 2024-05-21 21:17:55.233502 swarms-5.0.5/swarms/tools/base_tool.py
+-rw-r--r--   0        0        0     6653 2024-05-20 23:12:19.595923 swarms-5.0.5/swarms/tools/code_interpreter.py
+-rw-r--r--   0        0        0     5367 2024-05-20 23:12:19.595980 swarms-5.0.5/swarms/tools/exec_tool.py
+-rw-r--r--   0        0        0      773 2024-05-20 23:12:19.596031 swarms-5.0.5/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-05-20 23:12:19.596094 swarms-5.0.5/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-05-20 23:12:19.596178 swarms-5.0.5/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-05-20 23:12:19.596226 swarms-5.0.5/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0     1461 2024-05-20 23:12:19.596276 swarms-5.0.5/swarms/tools/math_eval.py
+-rw-r--r--   0        0        0      978 2024-05-20 23:12:19.596325 swarms-5.0.5/swarms/tools/openai_func_calling_schema.py
+-rw-r--r--   0        0        0    13875 2024-05-20 23:12:19.596409 swarms-5.0.5/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0    15564 2024-05-20 23:12:19.596483 swarms-5.0.5/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     4275 2024-05-20 23:12:19.596541 swarms-5.0.5/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0      157 2024-05-20 23:12:19.596586 swarms-5.0.5/swarms/tools/tool.py
+-rw-r--r--   0        0        0     6170 2024-05-20 23:12:19.596668 swarms-5.0.5/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-05-20 23:12:19.596758 swarms-5.0.5/swarms/utils/README.md
+-rw-r--r--   0        0        0     1956 2024-05-20 23:12:19.596815 swarms-5.0.5/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-05-20 23:12:19.596872 swarms-5.0.5/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-05-20 23:12:19.596962 swarms-5.0.5/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-05-20 23:12:19.597020 swarms-5.0.5/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-05-20 23:12:19.597075 swarms-5.0.5/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-05-20 23:12:19.597130 swarms-5.0.5/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-05-20 23:12:19.597203 swarms-5.0.5/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-05-20 23:12:19.597263 swarms-5.0.5/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-05-20 23:12:19.597318 swarms-5.0.5/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-05-20 23:12:19.597370 swarms-5.0.5/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-05-20 23:12:19.597441 swarms-5.0.5/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-05-20 23:12:19.597496 swarms-5.0.5/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-05-20 23:12:19.597550 swarms-5.0.5/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-05-20 23:12:19.597606 swarms-5.0.5/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-05-20 23:12:19.597693 swarms-5.0.5/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-05-20 23:12:19.597767 swarms-5.0.5/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     4232 2024-05-20 23:12:19.597842 swarms-5.0.5/swarms/utils/get_total_gpus.py
+-rw-r--r--   0        0        0     2848 2024-05-20 23:12:19.597905 swarms-5.0.5/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-05-20 23:12:19.597994 swarms-5.0.5/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-05-20 23:12:19.598063 swarms-5.0.5/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-05-20 23:12:19.598133 swarms-5.0.5/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-05-20 23:12:19.598202 swarms-5.0.5/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-05-20 23:12:19.598285 swarms-5.0.5/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-05-20 23:12:19.598349 swarms-5.0.5/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0      600 2024-05-20 23:12:19.598408 swarms-5.0.5/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-05-20 23:12:19.598470 swarms-5.0.5/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-05-20 23:12:19.598561 swarms-5.0.5/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-05-20 23:12:19.598619 swarms-5.0.5/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-05-20 23:12:19.598696 swarms-5.0.5/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-05-20 23:12:19.598755 swarms-5.0.5/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-05-20 23:12:19.598843 swarms-5.0.5/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    35219 1970-01-01 00:00:00.000000 swarms-5.0.5/PKG-INFO
```

### Comparing `swarms-5.0.3/LICENSE` & `swarms-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/README.md` & `swarms-5.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,64 @@
+Metadata-Version: 2.1
+Name: swarms
+Version: 5.0.5
+Summary: Swarms - Pytorch
+Home-page: https://github.com/kyegomez/swarms
+License: MIT
+Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
+Author: Kye Gomez
+Author-email: kye@apac.ai
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: Pillow (==10.3.0)
+Requires-Dist: PyYAML
+Requires-Dist: asyncio (>=3.4.3,<4.0)
+Requires-Dist: backoff (==2.2.1)
+Requires-Dist: docstring_parser (==0.16)
+Requires-Dist: langchain-community (==0.0.29)
+Requires-Dist: langchain-experimental (==0.0.55)
+Requires-Dist: loguru (==0.7.2)
+Requires-Dist: opencv-python-headless
+Requires-Dist: psutil
+Requires-Dist: pydantic (==2.7.1)
+Requires-Dist: pypdf (==4.1.0)
+Requires-Dist: python-dotenv
+Requires-Dist: ratelimit (==2.2.1)
+Requires-Dist: sentry-sdk
+Requires-Dist: tenacity (==8.2.3)
+Requires-Dist: toml
+Requires-Dist: torch (>=2.1.1,<3.0)
+Requires-Dist: transformers (>=4.39.0,<5.0.0)
+Project-URL: Documentation, https://swarms.world
+Project-URL: Repository, https://github.com/kyegomez/swarms
+Description-Content-Type: text/markdown
+
 ![Swarming banner icon](images/swarmslogobanner.png)
 
 <div align="center">
 
 Orchestrate swarms of agents for production-grade applications.
 
 [![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)
 
 [![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 </div>
 
-Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.
+
+Individual agents face 5 significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.
 ----
 
 ## Install
 `$ pip3 install -U swarms==4.9.7`
 
 ---
 
@@ -582,58 +624,14 @@
 
 # Run the workflow
 workflow.run()
 ```
 
 
 
-### `ModelParallelizer`
-The ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.
-
-Plug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.
-
-
-```python
-import os
-
-from dotenv import load_dotenv
-
-from swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat
-
-load_dotenv()
-
-# API Keys
-anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
-openai_api_key = os.getenv("OPENAI_API_KEY")
-gemini_api_key = os.getenv("GEMINI_API_KEY")
-
-# Initialize the models
-llm = OpenAIChat(openai_api_key=openai_api_key)
-anthropic = Anthropic(anthropic_api_key=anthropic_api_key)
-mixtral = Mixtral()
-gemini = Gemini(gemini_api_key=gemini_api_key)
-
-# Initialize the parallelizer
-llms = [llm, anthropic, mixtral, gemini]
-parallelizer = ModelParallelizer(llms)
-
-# Set the task
-task = "Generate a 10,000 word blog on health and wellness."
-
-# Run the task
-out = parallelizer.run(task)
-
-# Print the responses 1 by 1
-for i in range(len(out)):
-    print(f"Response from LLM {i}: {out[i]}")
-```
-
-
-
-
 ### `SwarmNetwork`
 `SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.
 
 ✅ Efficient Task Management: SwarmNetwork's intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.
 
 ✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.
 
@@ -752,114 +750,14 @@
 print(f"Task result: {task.result}")
 ```
 
 ---
 
 
 
-### `BlockList`
-- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.
-
-- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.
-
-- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.
-
-```python
-import os
-
-from dotenv import load_dotenv
-from transformers import AutoModelForCausalLM, AutoTokenizer
-from pydantic import BaseModel
-from swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent
-
-# Load the environment variables
-load_dotenv()
-
-# Get the environment variables
-openai_api_key = os.getenv("OPENAI_API_KEY")
-gemini_api_key = os.getenv("GEMINI_API_KEY")
-
-# Tool Agent
-model = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")
-tokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")
-
-# Initialize the schema for the person's information
-class Schema(BaseModel):
-    name: str = Field(..., title="Name of the person")
-    agent: int = Field(..., title="Age of the person")
-    is_student: bool = Field(
-        ..., title="Whether the person is a student"
-    )
-    courses: list[str] = Field(
-        ..., title="List of courses the person is taking"
-    )
-
-# Convert the schema to a JSON string
-json_schema = base_model_to_json(Schema)
-
-
-toolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)
-
-# Blocks List which enables you to build custom swarms by adding classes or functions
-swarm = BlocksList(
-    "SocialMediaSwarm",
-    "A swarm of social media agents",
-    [
-        OpenAI(openai_api_key=openai_api_key),
-        Mixtral(),
-        GPT4VisionAPI(openai_api_key=openai_api_key),
-        Gemini(gemini_api_key=gemini_api_key),
-    ],
-)
-
-
-# Add the new block to the swarm
-swarm.add(toolagent)
-
-# Remove a block from the swarm
-swarm.remove(toolagent)
-
-# Update a block in the swarm
-swarm.update(toolagent)
-
-# Get a block at a specific index
-block_at_index = swarm.get(0)
-
-# Get all blocks in the swarm
-all_blocks = swarm.get_all()
-
-# Get blocks by name
-openai_blocks = swarm.get_by_name("OpenAI")
-
-# Get blocks by type
-gpt4_blocks = swarm.get_by_type("GPT4VisionAPI")
-
-# Get blocks by ID
-block_by_id = swarm.get_by_id(toolagent.id)
-
-# Get blocks by parent
-blocks_by_parent = swarm.get_by_parent(swarm)
-
-# Get blocks by parent ID
-blocks_by_parent_id = swarm.get_by_parent_id(swarm.id)
-
-# Get blocks by parent name
-blocks_by_parent_name = swarm.get_by_parent_name(swarm.name)
-
-# Get blocks by parent type
-blocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)
-
-# Get blocks by parent description
-blocks_by_parent_description = swarm.get_by_parent_description(swarm.description)
-
-# Run the block in the swarm
-inference = swarm.run_block(toolagent, "Hello World")
-print(inference)
-```
-
 
 ## Majority Voting
 Multiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)
 
 ```python
 from swarms import Agent, MajorityVoting, ChromaDB, Anthropic
 
@@ -1244,30 +1142,34 @@
     "Create a format to express and communicate swarms of llms in a structured manner for youtube",
 )
 
 print(output)
 
 ```
 
+## `HierarhicalSwarm`
+Coming soon...
+
 
 ---
 
 ## Documentation
 Documentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)
 
 ----
 
-## File Structure
+## Folder Structure
 The swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs` that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.
 
 ```sh
 ├── __init__.py
 ├── agents
 ├── artifacts
 ├── memory
+├── schemas
 ├── models
 ├── prompts
 ├── structs
 ├── telemetry
 ├── tools
 ├── utils
 └── workers
@@ -1308,21 +1210,30 @@
 ## Accelerate Backlog
 Accelerate Bugs, Features, and Demos to implement by supporting us here:
 
 <a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>
 
 
 ## Docker Instructions
-- [Learn More Here About Deployments In Docker]()
+- [Learn More Here About Deployments In Docker](https://swarms.apac.ai/en/latest/docker_setup/)
 
 
 ## Swarm Newsletter 🤖 🤖 🤖 📧 
 Sign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊
 
-
 [CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)
 
 # License
 Apache License
 
-
+# Citation
+Please cite Swarms in your paper or your project if you found it beneficial in any way! Appreciate you.
+```bibtex
+@misc{swarms,
+  author = {Gomez, Kye},
+  title = {{Swarms: The Multi-Agent Collaboration Framework}},
+  howpublished = {\url{https://github.com/kyegomez/swarms}},
+  year = {2023},
+  note = {Accessed: Date}
+}
+```
```

### Comparing `swarms-5.0.3/pyproject.toml` & `swarms-5.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "5.0.3"
+version = "5.0.5"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
 documentation = "https://swarms.world"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
@@ -50,15 +50,15 @@
 python-dotenv = "*"
 opencv-python-headless = "*"
 PyYAML = "*"
 docstring_parser = "0.16"
 
 [tool.poetry.group.lint.dependencies]
 black = ">=23.1,<25.0"
-ruff = ">=0.0.249,<0.4.3"
+ruff = ">=0.0.249,<0.4.5"
 types-toml = "^0.10.8.1"
 types-pytz = ">=2023.3,<2025.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `swarms-5.0.3/swarms/__init__.py` & `swarms-5.0.5/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/__init__.py` & `swarms-5.0.5/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/agent_wrapper.py` & `swarms-5.0.5/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/base.py` & `swarms-5.0.5/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/developer_agents.py` & `swarms-5.0.5/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/omni_modal_agent.py` & `swarms-5.0.5/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/simple_agent.py` & `swarms-5.0.5/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/tool_agent.py` & `swarms-5.0.5/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/agents/worker_agent.py` & `swarms-5.0.5/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/artifacts/base_artifact.py` & `swarms-5.0.5/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/artifacts/text_artifact.py` & `swarms-5.0.5/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/__init__.py` & `swarms-5.0.5/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/base_db.py` & `swarms-5.0.5/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/base_vectordb.py` & `swarms-5.0.5/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/dict_internal_memory.py` & `swarms-5.0.5/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/dict_shared_memory.py` & `swarms-5.0.5/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/short_term_memory.py` & `swarms-5.0.5/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/memory/visual_memory.py` & `swarms-5.0.5/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/__init__.py` & `swarms-5.0.5/swarms/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from swarms.models.fuyu import Fuyu  # noqa: E402
 from swarms.models.gpt4_vision_api import GPT4VisionAPI  # noqa: E402
 from swarms.models.huggingface import HuggingfaceLLM  # noqa: E402
 from swarms.models.idefics import Idefics  # noqa: E402
 from swarms.models.kosmos_two import Kosmos  # noqa: E402
 from swarms.models.layoutlm_document_qa import LayoutLMDocumentQA
 from swarms.models.llava import LavaMultiModal  # noqa: E402
-from swarms.models.mistral import Mistral  # noqa: E402
-from swarms.models.mixtral import Mixtral  # noqa: E402
+
 from swarms.models.nougat import Nougat  # noqa: E402
 from swarms.models.palm import GooglePalm as Palm  # noqa: E402
 from swarms.models.openai_tts import OpenAITTS  # noqa: E402
 from swarms.models.popular_llms import Anthropic as Anthropic
 from swarms.models.popular_llms import (
     AzureOpenAILLM as AzureOpenAI,
 )
@@ -49,16 +48,14 @@
     "Fuyu",
     "GPT4VisionAPI",
     "HuggingfaceLLM",
     "Idefics",
     "Kosmos",
     "LayoutLMDocumentQA",
     "LavaMultiModal",
-    "Mistral",
-    "Mixtral",
     "Nougat",
     "Palm",
     "OpenAITTS",
     "Anthropic",
     "AzureOpenAI",
     "Cohere",
     "OpenAIChat",
```

### Comparing `swarms-5.0.3/swarms/models/base_embedding_model.py` & `swarms-5.0.5/swarms/models/base_embedding_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
                 else:
                     return self.try_embed_chunk(string)
 
         else:
             raise RuntimeError("Failed to embed string.")
 
     @abstractmethod
-    def try_embed_chunk(self, chunk: str) -> list[float]:
-        ...
+    def try_embed_chunk(self, chunk: str) -> list[float]: ...
 
     def _embed_long_string(self, string: str) -> list[float]:
         """Embeds a string that is too long to embed in one go."""
         chunks = self.chunker.chunk(string)
 
         embedding_chunks = []
         length_chunks = []
```

### Comparing `swarms-5.0.3/swarms/models/base_llm.py` & `swarms-5.0.5/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/base_multimodal_model.py` & `swarms-5.0.5/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/base_tts.py` & `swarms-5.0.5/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/base_ttv.py` & `swarms-5.0.5/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/cog_vlm.py` & `swarms-5.0.5/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/dalle3.py` & `swarms-5.0.5/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/distilled_whisperx.py` & `swarms-5.0.5/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/embeddings_base.py` & `swarms-5.0.5/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/fuyu.py` & `swarms-5.0.5/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/gemini.py` & `swarms-5.0.5/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/gpt4_vision_api.py` & `swarms-5.0.5/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/huggingface.py` & `swarms-5.0.5/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/huggingface_pipeline.py` & `swarms-5.0.5/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/idefics.py` & `swarms-5.0.5/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/kosmos_two.py` & `swarms-5.0.5/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/layoutlm_document_qa.py` & `swarms-5.0.5/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/llama3_hosted.py` & `swarms-5.0.5/swarms/models/llama3_hosted.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import json
-from swarms import BaseLLM
+from swarms.models.base_llm import BaseLLM
 
 
 class llama3Hosted(BaseLLM):
     """
     A class representing a hosted version of the Llama3 model.
 
     Args:
@@ -28,35 +28,36 @@
 
     def __init__(
         self,
         model: str = "meta-llama/Meta-Llama-3-8B-Instruct",
         temperature: float = 0.8,
         max_tokens: int = 4000,
         system_prompt: str = "You are a helpful assistant.",
+        base_url: str = "http://34.204.8.31:30001/v1/chat/completions",
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.model = model
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.system_prompt = system_prompt
+        self.base_url = base_url
 
     def run(self, task: str, *args, **kwargs) -> str:
         """
         Generates a response for the given task.
 
         Args:
             task (str): The user's task or input.
 
         Returns:
             str: The generated response from the Llama3 model.
 
         """
-        url = "http://34.204.8.31:30001/v1/chat/completions"
 
         payload = json.dumps(
             {
                 "model": self.model,
                 "messages": [
                     {"role": "system", "content": self.system_prompt},
                     {"role": "user", "content": task},
@@ -66,15 +67,15 @@
                 "max_tokens": self.max_tokens,
             }
         )
 
         headers = {"Content-Type": "application/json"}
 
         response = requests.request(
-            "POST", url, headers=headers, data=payload
+            "POST", self.base_url, headers=headers, data=payload
         )
 
         response_json = response.json()
         assistant_message = response_json["choices"][0]["message"][
             "content"
         ]
```

### Comparing `swarms-5.0.3/swarms/models/llama_function_caller.py` & `swarms-5.0.5/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/llava.py` & `swarms-5.0.5/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/mixtral.py` & `swarms-5.0.5/swarms/models/open_dalle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,67 @@
-from typing import Optional
+from typing import Any, Optional
 
-from transformers import AutoModelForCausalLM, AutoTokenizer
+import torch
+from diffusers import AutoPipelineForText2Image
 
-from swarms.models.base_llm import BaseLLM
+from swarms.models.base_multimodal_model import BaseMultiModalModel
 
 
-class Mixtral(BaseLLM):
-    """Mixtral model.
-
-    Args:
-        model_name (str): The name or path of the pre-trained Mixtral model.
-        max_new_tokens (int): The maximum number of new tokens to generate.
-        *args: Variable length argument list.
+class OpenDalle(BaseMultiModalModel):
+    """OpenDalle model class
 
+    Attributes:
+        model_name (str): The name or path of the model to be used. Defaults to "dataautogpt3/OpenDalleV1.1".
+        torch_dtype (torch.dtype): The torch data type to be used. Defaults to torch.float16.
+        device (str): The device to be used for computation. Defaults to "cuda".
 
     Examples:
-        >>> from swarms.models import Mixtral
-        >>> mixtral = Mixtral()
-        >>> mixtral.run("Test task")
-        'Generated text'
+        >>> from swarms.models.open_dalle import OpenDalle
+        >>> od = OpenDalle()
+        >>> od.run("A picture of a cat")
+
     """
 
     def __init__(
         self,
-        model_name: str = "mistralai/Mixtral-8x7B-v0.1",
-        max_new_tokens: int = 500,
+        model_name: str = "dataautogpt3/OpenDalleV1.1",
+        torch_dtype: Any = torch.float16,
+        device: str = "cuda",
         *args,
         **kwargs,
     ):
         """
-        Initializes a Mixtral model.
+        Initializes the OpenDalle model.
 
         Args:
-            model_name (str): The name or path of the pre-trained Mixtral model.
-            max_new_tokens (int): The maximum number of new tokens to generate.
+            model_name (str, optional): The name or path of the model to be used. Defaults to "dataautogpt3/OpenDalleV1.1".
+            torch_dtype (torch.dtype, optional): The torch data type to be used. Defaults to torch.float16.
+            device (str, optional): The device to be used for computation. Defaults to "cuda".
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
         """
-        super().__init__(*args, **kwargs)
-        self.model_name = model_name
-        self.max_new_tokens = max_new_tokens
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name)
-        self.model = AutoModelForCausalLM.from_pretrained(
-            model_name, *args, **kwargs
-        )
+        self.pipeline = AutoPipelineForText2Image.from_pretrained(
+            model_name, torch_dtype=torch_dtype, *args, **kwargs
+        ).to(device)
 
-    def run(self, task: Optional[str] = None, **kwargs):
-        """
-        Generates text based on the given task.
+    def run(self, task: Optional[str] = None, *args, **kwargs):
+        """Run the OpenDalle model
 
         Args:
-            task (str, optional): The task or prompt for text generation.
+            task (str, optional): The task to be performed. Defaults to None.
+            *args: Variable length argument list.
+            **kwargs: Arbitrary keyword arguments.
 
         Returns:
-            str: The generated text.
+            [type]: [description]
         """
         try:
-            inputs = self.tokenizer(task, return_tensors="pt")
-
-            outputs = self.model.generate(
-                **inputs,
-                max_new_tokens=self.max_new_tokens,
-                **kwargs,
-            )
-
-            out = self.tokenizer.decode(
-                outputs[0],
-                skip_special_tokens=True,
-            )
-
-            return out
+            if task is None:
+                raise ValueError("Task cannot be None")
+            if not isinstance(task, str):
+                raise TypeError("Task must be a string")
+            if len(task) < 1:
+                raise ValueError("Task cannot be empty")
+            return self.pipeline(task, *args, **kwargs).images[0]
         except Exception as error:
-            print(f"There is an error: {error} in Mixtral model.")
+            print(f"[ERROR][OpenDalle] {error}")
             raise error
```

### Comparing `swarms-5.0.3/swarms/models/moondream_mm.py` & `swarms-5.0.5/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/nougat.py` & `swarms-5.0.5/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/open_router.py` & `swarms-5.0.5/swarms/models/open_router.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/openai_tts.py` & `swarms-5.0.5/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/popular_llms.py` & `swarms-5.0.5/swarms/models/popular_llms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/qwen.py` & `swarms-5.0.5/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/sam.py` & `swarms-5.0.5/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/sampling_params.py` & `swarms-5.0.5/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/ssd_1b.py` & `swarms-5.0.5/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/together.py` & `swarms-5.0.5/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/types.py` & `swarms-5.0.5/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/vilt.py` & `swarms-5.0.5/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/vip_llava.py` & `swarms-5.0.5/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/models/zeroscope.py` & `swarms-5.0.5/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/__init__.py` & `swarms-5.0.5/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/accountant_swarm_prompts.py` & `swarms-5.0.5/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/aga.py` & `swarms-5.0.5/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/agent_output_parser.py` & `swarms-5.0.5/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/agent_prompt.py` & `swarms-5.0.5/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/agent_prompts.py` & `swarms-5.0.5/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/agent_system_prompts.py` & `swarms-5.0.5/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/ai_research_team.py` & `swarms-5.0.5/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/aot_prompt.py` & `swarms-5.0.5/swarms/prompts/aot_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/autobloggen.py` & `swarms-5.0.5/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/autoswarm.py` & `swarms-5.0.5/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/base.py` & `swarms-5.0.5/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/chat_prompt.py` & `swarms-5.0.5/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/code_interpreter.py` & `swarms-5.0.5/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/code_spawner.py` & `swarms-5.0.5/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/debate.py` & `swarms-5.0.5/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/documentation.py` & `swarms-5.0.5/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/education.py` & `swarms-5.0.5/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/finance_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/growth_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/idea2img.py` & `swarms-5.0.5/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/legal_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/logistics.py` & `swarms-5.0.5/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/meta_system_prompt.py` & `swarms-5.0.5/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-5.0.5/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/multi_modal_prompts.py` & `swarms-5.0.5/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-5.0.5/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/operations_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/personal_stylist.py` & `swarms-5.0.5/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/product_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/programming.py` & `swarms-5.0.5/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/project_manager.py` & `swarms-5.0.5/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/python.py` & `swarms-5.0.5/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/react.py` & `swarms-5.0.5/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/sales.py` & `swarms-5.0.5/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/sales_prompts.py` & `swarms-5.0.5/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/security_team.py` & `swarms-5.0.5/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/self_operating_prompt.py` & `swarms-5.0.5/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/summaries_prompts.py` & `swarms-5.0.5/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/support_agent_prompt.py` & `swarms-5.0.5/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/swarm_manager_agent.py` & `swarms-5.0.5/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/task_assignment_prompt.py` & `swarms-5.0.5/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/tests.py` & `swarms-5.0.5/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/tools.py` & `swarms-5.0.5/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/urban_planning.py` & `swarms-5.0.5/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/visual_cot.py` & `swarms-5.0.5/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/worker_prompt.py` & `swarms-5.0.5/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/prompts/xray_swarm_prompt.py` & `swarms-5.0.5/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/__init__.py` & `swarms-5.0.5/swarms/structs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,46 +4,48 @@
     AgentProcess,
     AgentProcessQueue,
 )
 from swarms.structs.auto_swarm import AutoSwarm, AutoSwarmRouter
 from swarms.structs.base_structure import BaseStructure
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.structs.base_workflow import BaseWorkflow
-from swarms.structs.block_wrapper import block
 from swarms.structs.concurrent_workflow import ConcurrentWorkflow
 from swarms.structs.conversation import Conversation
 from swarms.structs.groupchat import GroupChat, GroupChatManager
+from swarms.structs.hiearchical_swarm import HiearchicalSwarm
 from swarms.structs.majority_voting import (
     MajorityVoting,
     majority_voting,
     most_frequent,
     parse_code_completion,
 )
 from swarms.structs.message import Message
-from swarms.structs.model_parallizer import ModelParallelizer
+from swarms.structs.message_pool import MessagePool
 from swarms.structs.multi_agent_collab import MultiAgentCollaboration
 from swarms.structs.multi_process_workflow import (
     MultiProcessWorkflow,
 )
 from swarms.structs.multi_threaded_workflow import (
     MultiThreadedWorkflow,
 )
-from swarms.structs.plan import Plan
+from swarms.schemas.plan import Plan
+from swarms.structs.rearrange import AgentRearrange, rearrange
 from swarms.structs.recursive_workflow import RecursiveWorkflow
-from swarms.structs.schemas import (
+from swarms.structs.round_robin import RoundRobinSwarm
+from swarms.schemas.schemas import (
     Artifact,
     ArtifactUpload,
     StepInput,
     StepOutput,
     StepRequestBody,
     TaskInput,
     TaskRequestBody,
 )
 from swarms.structs.sequential_workflow import SequentialWorkflow
-from swarms.structs.step import Step
+from swarms.schemas.step import Step
 from swarms.structs.swarm_net import SwarmNetwork
 from swarms.structs.swarming_architectures import (
     broadcast,
     circular_swarm,
     exponential_swarm,
     fibonacci_swarm,
     geometric_swarm,
@@ -71,47 +73,40 @@
     distribute_tasks,
     extract_key_from_json,
     extract_tokens_from_text,
     find_agent_by_id,
     find_token_in_text,
     parse_tasks,
 )
-from swarms.structs.rearrange import AgentRearrange, rearrange
-
 from swarms.structs.yaml_model import (
-    get_type_name,
+    YamlModel,
     create_yaml_schema_from_dict,
+    get_type_name,
     pydantic_type_to_yaml_schema,
-    YamlModel,
 )
-from swarms.structs.message_pool import MessagePool
-from swarms.structs.round_robin import RoundRobinSwarm
-from swarms.structs.hiearchical_swarm import HiearchicalSwarm
 
 __all__ = [
     "Agent",
     "AgentJob",
     "AgentProcess",
     "AgentProcessQueue",
     "AutoSwarm",
     "AutoSwarmRouter",
     "BaseStructure",
     "BaseSwarm",
     "BaseWorkflow",
-    "block",
     "ConcurrentWorkflow",
     "Conversation",
     "GroupChat",
     "GroupChatManager",
     "MajorityVoting",
     "majority_voting",
     "most_frequent",
     "parse_code_completion",
     "Message",
-    "ModelParallelizer",
     "MultiAgentCollaboration",
     "MultiProcessWorkflow",
     "MultiThreadedWorkflow",
     "Plan",
     "RecursiveWorkflow",
     "Artifact",
     "ArtifactUpload",
@@ -155,9 +150,9 @@
     "get_type_name",
     "create_yaml_schema_from_dict",
     "pydantic_type_to_yaml_schema",
     "YamlModel",
     "MessagePool",
     "rearrange",
     "RoundRobinSwarm",
-    "HiearchicalSwarm"
+    "HiearchicalSwarm",
 ]
```

### Comparing `swarms-5.0.3/swarms/structs/agent.py` & `swarms-5.0.5/swarms/structs/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import os
 import random
 import sys
 import time
 import uuid
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
 import yaml
 from loguru import logger
 from pydantic import BaseModel
 from termcolor import colored
 
 from swarms.memory.base_vectordb import BaseVectorDatabase
 from swarms.prompts.agent_system_prompts import AGENT_SYSTEM_PROMPT_3
```

### Comparing `swarms-5.0.3/swarms/structs/agent_job.py` & `swarms-5.0.5/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/agent_process.py` & `swarms-5.0.5/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/async_workflow.py` & `swarms-5.0.5/swarms/structs/async_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
 from dataclasses import dataclass, field
 from typing import Any, Callable, List, Optional
 
 from swarms.structs.agent import Agent
 from swarms.structs.task import Task
 from swarms.utils.logger import logger
+from swarms.structs.base_swarm import BaseSwarm
 
 
 @dataclass
-class AsyncWorkflow:
+class AsyncWorkflow(BaseSwarm):
     """
     Represents an asynchronous workflow to run tasks.
 
     Attributes:
         name (str): The name of the workflow.
         description (str): The description of the workflow.
         max_loops (int): The maximum number of loops to run the workflow.
```

### Comparing `swarms-5.0.3/swarms/structs/auto_swarm.py` & `swarms-5.0.5/swarms/structs/auto_swarm.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,24 +112,27 @@
         name: Optional[str] = None,
         description: Optional[str] = None,
         verbose: bool = False,
         custom_params: Optional[Dict[str, Any]] = None,
         custom_preprocess: Optional[Callable] = None,
         custom_postprocess: Optional[Callable] = None,
         custom_router: Optional[Callable] = None,
+        max_loops: int = 1,
         *args,
         **kwargs,
     ):
         super().__init__()
         self.name = name
         self.description = description
         self.verbose = verbose
         self.custom_params = custom_params
         self.custom_preprocess = custom_preprocess
         self.custom_postprocess = custom_postprocess
+        self.custom_router = custom_router
+        self.max_loops = max_loops
         self.router = AutoSwarmRouter(
             name=name,
             description=description,
             verbose=verbose,
             custom_params=custom_params,
             custom_preprocess=custom_preprocess,
             custom_postprocess=custom_postprocess,
@@ -137,13 +140,38 @@
             *args,
             **kwargs,
         )
 
     def run(self, task: str = None, *args, **kwargs):
         """Run the swarm simulation."""
         try:
-            return self.router.run(task, *args, **kwargs)
+            loop = 0
+
+            while loop < self.max_loops:
+                if self.custom_preprocess:
+                    # If custom preprocess function is provided then run it
+                    logger.info("Running custom preprocess function.")
+                    task, args, kwargs = self.custom_preprocess(
+                        task, args, kwargs
+                    )
+
+                if self.custom_router:
+                    # If custom router function is provided then use it to route the task
+                    logger.info("Running custom router function.")
+                    out = self.custom_router(self, task, *args, **kwargs)
+
+                else:
+                    out = self.router.run(task, *args, **kwargs)
+
+                if self.custom_postprocess:
+                    # If custom postprocess function is provided then run it
+                    out = self.custom_postprocess(out)
+
+                # LOOP
+                loop += 1
+
+                return out
         except Exception as e:
             logger.error(
                 f"Error: {e} try optimizing the inputs and try again."
             )
             raise e
```

### Comparing `swarms-5.0.3/swarms/structs/base_structure.py` & `swarms-5.0.5/swarms/structs/base_structure.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/base_swarm.py` & `swarms-5.0.5/swarms/structs/base_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/base_workflow.py` & `swarms-5.0.5/swarms/structs/base_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/company.py` & `swarms-5.0.5/swarms/structs/company.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Union
 
 from swarms.structs.agent import Agent
 from swarms.structs.conversation import Conversation
 from swarms.utils.logger import logger
+from swarms.structs.base_swarm import BaseSwarm
 
 
 @dataclass
-class Company:
+class Company(BaseSwarm):
     """
     Represents a company with a hierarchical organizational structure.
     """
 
     org_chart: List[List[Agent]]
     shared_instructions: str = None
     ceo: Optional[Agent] = None
```

### Comparing `swarms-5.0.3/swarms/structs/concurrent_workflow.py` & `swarms-5.0.5/swarms/structs/concurrent_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import concurrent.futures
 from dataclasses import dataclass, field
 from typing import Callable, Dict, List, Optional
 
-from swarms.structs.base_structure import BaseStructure
 from swarms.structs.task import Task
 from swarms.utils.logger import logger
+from swarms.structs.agent import Agent
+from swarms.structs.base_workflow import BaseWorkflow
 
 
 @dataclass
-class ConcurrentWorkflow(BaseStructure):
+class ConcurrentWorkflow(BaseWorkflow):
     """
     ConcurrentWorkflow class for running a set of tasks concurrently using N number of autonomous agents.
 
     Args:
         max_workers (int): The maximum number of workers to use for the ThreadPoolExecutor.
         autosave (bool): Whether to save the state of the workflow to a file. Default is False.
         saved_state_filepath (str): The filepath to save the state of the workflow to. Default is "runs/concurrent_workflow.json".
@@ -31,21 +32,27 @@
     >>> workflow.tasks
     """
 
     task_pool: List[Dict] = field(default_factory=list)
     max_loops: int = 1
     max_workers: int = 5
     autosave: bool = False
+    agents: List[Agent] = None
     saved_state_filepath: Optional[str] = "runs/concurrent_workflow.json"
     print_results: bool = False
     return_results: bool = False
     use_processes: bool = False
     stopping_condition: Optional[Callable] = None
 
-    def add(self, task: Task = None, tasks: List[Task] = None):
+    def add(
+        self,
+        task: Task = None,
+        agent: Agent = None,
+        tasks: List[Task] = None,
+    ):
         """Adds a task to the workflow.
 
         Args:
             task (Task): _description_
             tasks (List[Task]): _description_
         """
         try:
@@ -57,31 +64,35 @@
                     )
             else:
                 if task:
                     self.task_pool.append(task)
                     logger.info(
                         f"Added task {task} to ConcurrentWorkflow."
                     )
+
+            if agent:
+                self.agents.append(agent)
+                logger.info(f"Added agent {agent} to ConcurrentWorkflow.")
         except Exception as error:
             logger.warning(f"[ERROR][ConcurrentWorkflow] {error}")
             raise error
 
-    def run(self, *args, **kwargs):
+    def run(self, task: str = None, *args, **kwargs):
         """
         Executes the tasks in parallel using a ThreadPoolExecutor.
 
         Args:
             print_results (bool): Whether to print the results of each task. Default is False.
             return_results (bool): Whether to return the results of each task. Default is False.
 
         Returns:
             List[Any]: A list of the results of each task, if return_results is True. Otherwise, returns None.
         """
-        loop_count = 0
-        while loop_count < self.max_loops:
+        loop = 0
+        while loop < self.max_loops:
             with concurrent.futures.ThreadPoolExecutor(
                 max_workers=self.max_workers
             ) as executor:
                 futures = {
                     executor.submit(task.execute): task
                     for task in self.task_pool
                 }
@@ -96,15 +107,15 @@
                         if self.return_results:
                             results.append(result)
                     except Exception as e:
                         logger.error(
                             f"Task {task} generated an exception: {e}"
                         )
 
-            loop_count += 1
+            loop += 1
             if self.stopping_condition and self.stopping_condition(
                 results
             ):
                 break
 
         return results if self.return_results else None
```

### Comparing `swarms-5.0.3/swarms/structs/conversation.py` & `swarms-5.0.5/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/debate.py` & `swarms-5.0.5/swarms/structs/debate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 from datetime import datetime
 from typing import List
 
 from swarms.structs.agent import Agent
+from swarms.structs.base_swarm import BaseSwarm
 
 NAME_LIST = [
     "Affirmative side",
     "Negative side",
     "Moderator",
 ]
 
@@ -22,15 +23,15 @@
             temperature (float): higher values make the output more random, while lower values make it more focused and deterministic
             openai_api_key (str): As the parameter name suggests
             sleep_time (float): sleep because of rate limits
         """
         super().__init__(llm=llm, agent_name=name, *args, **kwargs)
 
 
-class Debate:
+class Debate(BaseSwarm):
     """Create a debate
 
     Args:
         model_name (str): openai model name
         temperature (float): higher values make the output more random, while lower values make it more focused and deterministic
         num_players (int): num of players
         save_file_dir (str): dir path to json file
```

### Comparing `swarms-5.0.3/swarms/structs/groupchat.py` & `swarms-5.0.5/swarms/structs/groupchat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass, field
 from typing import List
 from swarms.structs.conversation import Conversation
 from swarms.utils.loguru_logger import logger
 from swarms.structs.agent import Agent
+from swarms.structs.base_swarm import BaseSwarm
 
 
 @dataclass
-class GroupChat:
+class GroupChat(BaseSwarm):
     """
     A group chat class that contains a list of agents and the maximum number of rounds.
 
     Args:
         agents: List[Agent]
         messages: List[Dict]
         max_round: int
```

### Comparing `swarms-5.0.3/swarms/structs/hiearchical_swarm.py` & `swarms-5.0.5/swarms/structs/hiearchical_swarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from swarms.structs.agent import Agent
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.utils.loguru_logger import logger
 
 
 class HiearchicalSwarm(BaseSwarm):
-    
     @beartype
     def __init__(
         self,
         director: Agent = None,
         agents: List[Agent] = None,
         max_loops: int = 1,
         long_term_memory_system: BaseSwarm = None,
@@ -21,24 +20,23 @@
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.director = director
         self.agents = agents
         self.max_loops = max_loops
         self.long_term_memory_system = long_term_memory_system
-        
+
         # Set the director to max_one loop
-        self.director.max_loops = 1
-        
+        if self.director.max_loops > 1:
+            self.director.max_loops = 1
+
         # Set the long term memory system of every agent to long term memory system
         if long_term_memory_system is True:
             for agent in agents:
                 agent.long_term_memory = long_term_memory_system
-                
-        
 
     def parse_function_activate_agent(
         self, json_data: str = None, *args, **kwargs
     ):
         """
         Parse the JSON data and activate the selected agent.
 
@@ -111,15 +109,15 @@
 
         Raises:
             Exception: If an error occurs while running the swarm.
 
         """
         try:
             loop = 0
-            
+
             # While the loop is less than max loops
             while loop < self.max_loops:
                 # Run the director
                 response = self.director.run(task, *args, **kwargs)
 
                 # Run agents
                 response = self.parse_function_activate_agent(response)
```

### Comparing `swarms-5.0.3/swarms/structs/majority_voting.py` & `swarms-5.0.5/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/message_pool.py` & `swarms-5.0.5/swarms/structs/message_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import hashlib
 from time import time_ns
 from typing import Callable, List, Optional, Sequence, Union
 
 from swarms.structs.agent import Agent
 from swarms.utils.loguru_logger import logger
+from swarms.structs.base_swarm import BaseSwarm
 
 
 def _hash(input: str):
     """
     Hashes the input string using SHA256 algorithm.
 
     Args:
@@ -38,15 +39,15 @@
     time = time_ns()
     return _hash(
         f"agent: {agent.agent_name}\ncontent: {content}\ntimestamp:"
         f" {str(time)}\nturn: {turn}\nmsg_type: {msg_type}"
     )
 
 
-class MessagePool:
+class MessagePool(BaseSwarm):
     """
     A class representing a message pool for agents in a swarm.
 
     Attributes:
         agents (Optional[Sequence[Agent]]): The list of agents in the swarm.
         moderator (Optional[Agent]): The moderator agent.
         turns (Optional[int]): The number of turns.
```

### Comparing `swarms-5.0.3/swarms/structs/meta_system_prompt.py` & `swarms-5.0.5/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/multi_agent_collab.py` & `swarms-5.0.5/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/multi_process_workflow.py` & `swarms-5.0.5/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/multi_threaded_workflow.py` & `swarms-5.0.5/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/rearrange.py` & `swarms-5.0.5/swarms/structs/rearrange.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import List
+from typing import Callable, Dict, List, Optional
+
 from swarms.memory.base_vectordb import BaseVectorDatabase
+from swarms.structs.agent import Agent
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.utils.loguru_logger import logger
-from typing import Optional, Callable, Dict
-from swarms.structs.omni_agent_types import Agent
-from swarms.structs.agent import Agent
 
 
 class AgentRearrange(BaseSwarm):
     """
     A class representing a swarm of agents for rearranging tasks.
 
     Attributes:
@@ -279,60 +278,7 @@
         task = "Perform a task"
         rearrange(agents, flow, task)
     """
     agent_system = AgentRearrange(
         agents=agents, flow=flow, *args, **kwargs
     )
     return agent_system.run(task, *args, **kwargs)
-
-
-# # Initialize the director agent
-# director = Agent(
-#     agent_name="Director",
-#     system_prompt="Directs the tasks for the workers",
-#     llm=Anthropic(),
-#     max_loops=1,
-#     dashboard=False,
-#     streaming_on=True,
-#     verbose=True,
-#     stopping_token="<DONE>",
-#     state_save_file_type="json",
-#     saved_state_path="director.json",
-# )
-
-# # Initialize worker 1
-# worker1 = Agent(
-#     agent_name="Worker1",
-#     system_prompt="Generates a transcript for a youtube video on what swarms are",
-#     llm=Anthropic(),
-#     max_loops=1,
-#     dashboard=False,
-#     streaming_on=True,
-#     verbose=True,
-#     stopping_token="<DONE>",
-#     state_save_file_type="json",
-#     saved_state_path="worker1.json",
-# )
-
-# # Initialize worker 2
-# worker2 = Agent(
-#     agent_name="Worker2",
-#     system_prompt="Summarizes the transcript generated by Worker1",
-#     llm=Anthropic(),
-#     max_loops=1,
-#     dashboard=False,
-#     streaming_on=True,
-#     verbose=True,
-#     stopping_token="<DONE>",
-#     state_save_file_type="json",
-#     saved_state_path="worker2.json",
-# )
-
-
-# flow = "Director -> Worker1 -> Worker2"
-# agent_system = AgentRearrange(
-#     agents=[director, worker1, worker2], flow=flow
-# )
-# # Run the system
-# output = agent_system.run(
-#     "Create a format to express and communicate swarms of llms in a structured manner for youtube"
-# )
```

### Comparing `swarms-5.0.3/swarms/structs/recursive_workflow.py` & `swarms-5.0.5/swarms/structs/recursive_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     >>> workflow.run()
     """
 
     def __init__(
         self,
         stop_token: str = "<DONE>",
         stopping_conditions: callable = None,
+        max_loops: int = 1,
+        *args,
+        **kwargs,
     ):
         self.stop_token = stop_token
         self.stopping_conditions = stopping_conditions
         self.task_pool = []
 
         assert self.stop_token is not None, "stop_token cannot be None"
 
@@ -71,16 +74,24 @@
         """
         Executes the tasks in the workflow until the stop token is encountered.
 
         Returns:
             None
         """
         try:
-            for task in self.task_pool:
-                while True:
-                    result = task.run()
-                    if result is not None and self.stop_token in result:
-                        break
-                    print(f"{result}")
+            loop = 0
+            while loop < self.max_loops:
+                for task in self.task_pool:
+                    while True:
+                        result = task.run()
+                        if (
+                            result is not None
+                            and self.stop_token in result
+                        ):
+                            break
+                        print(f"{result}")
+                loop += 1
+
+            return result
         except Exception as error:
             logger.warning(f"[ERROR][RecursiveWorkflow] {error}")
             raise error
```

### Comparing `swarms-5.0.3/swarms/structs/round_robin.py` & `swarms-5.0.5/swarms/structs/round_robin.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/schemas.py` & `swarms-5.0.5/swarms/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/sequential_workflow.py` & `swarms-5.0.5/swarms/structs/sequential_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/sermon_swarm.py` & `swarms-5.0.5/swarms/structs/sermon_swarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,20 +46,25 @@
         sermon = self.priest(task, *args, **kwargs)
 
         # Add the sermon to the memory of all agents
         for agent in self.agents:
             agent.add_message_to_memory(sermon)
 
         # Then run the agents
-        for _ in range(self.max_loops):
+        loop = 0
+        # for _ in range(self.max_loops):
+        while loop < self.max_loops:
             for agent in self.agents:
                 preach = agent.run(task, *args, **kwargs)
 
                 if self.stop_function:
                     preach = self.stop_function(preach)
 
                 if self.stop_condition in preach:
                     if self.stop_condition is True:
                         break
 
                     elif self.stop_condition in preach:
                         break
+
+            loop += 1
+            return preach
```

### Comparing `swarms-5.0.3/swarms/structs/step.py` & `swarms-5.0.5/swarms/schemas/step.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/swarm_net.py` & `swarms-5.0.5/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/swarming_architectures.py` & `swarms-5.0.5/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/task.py` & `swarms-5.0.5/swarms/structs/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Union
 
 from swarms.structs.agent import Agent
 from swarms.structs.conversation import Conversation
 from swarms.utils.logger import logger
+from swarms.structs.omni_agent_types import AgentType
 
 
 @dataclass
 class Task:
     """
     Task class for running a task in a sequential workflow.
 
@@ -47,15 +48,15 @@
     >>> agent = Agent(llm=OpenAIChat(openai_api_key=""), max_loops=1, dashboard=False)
     >>> task = Task(description="What's the weather in miami", agent=agent)
     >>> task.execute()
     >>> task.result
 
     """
 
-    agent: Union[Callable, Agent]
+    agent: Union[Callable, Agent, AgentType] = None
     description: str = None
     result: Any = None
     history: List[Any] = field(default_factory=list)
     schedule_time: datetime = None
     scheduler = sched.scheduler(time.time, time.sleep)
     trigger: Callable = None
     action: Callable = None
```

### Comparing `swarms-5.0.3/swarms/structs/task_queue_base.py` & `swarms-5.0.5/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/utils.py` & `swarms-5.0.5/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/structs/yaml_model.py` & `swarms-5.0.5/swarms/structs/yaml_model.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/telemetry/__init__.py` & `swarms-5.0.5/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-5.0.5/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/telemetry/check_update.py` & `swarms-5.0.5/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/telemetry/log_all.py` & `swarms-5.0.5/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/telemetry/sys_info.py` & `swarms-5.0.5/swarms/telemetry/sys_info.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/telemetry/user_utils.py` & `swarms-5.0.5/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/__init__.py` & `swarms-5.0.5/swarms/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/base_tool.py` & `swarms-5.0.5/swarms/tools/base_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,27 @@
     functions: List[Callable[..., Any]] = []
     base_models: List[type[BaseModel]] = []
     verbose: bool = False
     autocheck: bool = False
     auto_execute_tool: Optional[bool] = False
 
     def func_to_dict(
-        function: Callable[..., Any],
-        *,
+        function: Callable[..., Any] = None,
         name: Optional[str] = None,
-        description: str,
+        description: str = None,
+        *args,
+        **kwargs,
     ) -> Dict[str, Any]:
         try:
             return get_openai_function_schema_from_func(
                 function=function,
                 name=name,
                 description=description,
+                *args,
+                **kwargs,
             )
         except Exception as e:
             logger.error(f"An error occurred in func_to_dict: {e}")
             logger.error(
                 "Please check the function and ensure it is valid."
             )
             logger.error(
```

### Comparing `swarms-5.0.3/swarms/tools/code_interpreter.py` & `swarms-5.0.5/swarms/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/exec_tool.py` & `swarms-5.0.5/swarms/tools/exec_tool.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/function_util.py` & `swarms-5.0.5/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/json_former.py` & `swarms-5.0.5/swarms/tools/json_former.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/json_utils.py` & `swarms-5.0.5/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/logits_processor.py` & `swarms-5.0.5/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/math_eval.py` & `swarms-5.0.5/swarms/tools/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/openai_func_calling_schema.py` & `swarms-5.0.5/swarms/tools/openai_func_calling_schema.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/openai_tool_creator_decorator.py` & `swarms-5.0.5/swarms/tools/openai_tool_creator_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/py_func_to_openai_func_str.py` & `swarms-5.0.5/swarms/tools/py_func_to_openai_func_str.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/pydantic_to_json.py` & `swarms-5.0.5/swarms/tools/pydantic_to_json.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/tools/tool_utils.py` & `swarms-5.0.5/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/README.md` & `swarms-5.0.5/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/__init__.py` & `swarms-5.0.5/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/apa.py` & `swarms-5.0.5/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/check_function_result.py` & `swarms-5.0.5/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/class_args_wrapper.py` & `swarms-5.0.5/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/concurrent_utils.py` & `swarms-5.0.5/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/data_to_text.py` & `swarms-5.0.5/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/decorators.py` & `swarms-5.0.5/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/disable_logging.py` & `swarms-5.0.5/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/download_img.py` & `swarms-5.0.5/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/execute_futures.py` & `swarms-5.0.5/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/exponential_backoff.py` & `swarms-5.0.5/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/fetch_init_params.py` & `swarms-5.0.5/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/file_processing.py` & `swarms-5.0.5/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/find_img_path.py` & `swarms-5.0.5/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/get_logger.py` & `swarms-5.0.5/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/get_total_gpus.py` & `swarms-5.0.5/swarms/utils/get_total_gpus.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/json_output_parser.py` & `swarms-5.0.5/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/jsonl_utils.py` & `swarms-5.0.5/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/llm_metrics_decorator.py` & `swarms-5.0.5/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/logger.py` & `swarms-5.0.5/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/loggers.py` & `swarms-5.0.5/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/markdown_message.py` & `swarms-5.0.5/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/parse_code.py` & `swarms-5.0.5/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/pdf_to_text.py` & `swarms-5.0.5/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/remove_json_whitespace.py` & `swarms-5.0.5/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/save_logs.py` & `swarms-5.0.5/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/serializable.py` & `swarms-5.0.5/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/try_except_wrapper.py` & `swarms-5.0.5/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/swarms/utils/yaml_output_parser.py` & `swarms-5.0.5/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-5.0.3/setup.py` & `swarms-5.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,1197 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+![Swarming banner icon](images/swarmslogobanner.png)
 
-packages = \
-['swarms',
- 'swarms.agents',
- 'swarms.artifacts',
- 'swarms.memory',
- 'swarms.models',
- 'swarms.prebuilt_swarms',
- 'swarms.prompts',
- 'swarms.structs',
- 'swarms.telemetry',
- 'swarms.tools',
- 'swarms.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pillow==10.3.0',
- 'PyYAML',
- 'asyncio>=3.4.3,<4.0',
- 'backoff==2.2.1',
- 'docstring_parser==0.16',
- 'langchain-community==0.0.29',
- 'langchain-experimental==0.0.55',
- 'loguru==0.7.2',
- 'opencv-python-headless',
- 'psutil',
- 'pydantic==2.7.1',
- 'pypdf==4.1.0',
- 'python-dotenv',
- 'ratelimit==2.2.1',
- 'sentry-sdk',
- 'tenacity==8.2.3',
- 'toml',
- 'torch>=2.1.1,<3.0',
- 'transformers>=4.39.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'swarms',
-    'version': '5.0.3',
-    'description': 'Swarms - Pytorch',
-    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.\n----\n\n## Install\n`$ pip3 install -U swarms==4.9.7`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n## `Agent`with Pydantic BaseModel as Output Type\nThe following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:\n\n```python\nfrom pydantic import BaseModel, Field\nfrom swarms import Anthropic, Agent\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(..., title="Whether the person is a student")\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = Schema(\n    name="Tool Name",\n    agent=1,\n    is_student=True,\n    courses=["Course1", "Course2"],\n)\n\n# Define the task to generate a person\'s information\ntask = "Generate a person\'s information based on the following schema:"\n\n# Initialize the agent\nagent = Agent(\n    agent_name="Person Information Generator",\n    system_prompt=(\n        "Generate a person\'s information based on the following schema:"\n    ),\n    # Set the tool schema to the JSON string -- this is the key difference\n    tool_schema=tool_schema,\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    interactive=True,\n    # Set the output type to the tool schema which is a BaseModel\n    output_type=tool_schema,  # or dict, or str\n    metadata_output_type="json",\n    # List of schemas that the agent can handle\n    list_tool_schemas=[tool_schema],\n    function_calling_format_type="OpenAI",\n    function_calling_type="json",  # or soon yaml\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nfrom swarms import Agent, SequentialWorkflow, Anthropic\n\n\n# Initialize the language model agent (e.g., GPT-3)\nllm = Anthropic()\n\n# Initialize agents for individual tasks\nagent1 = Agent(\n    agent_name="Blog generator",\n    system_prompt="Generate a blog post like stephen king",\n    llm=llm,\n    max_loops=1,\n    dashboard=False,\n    tools=[],\n)\nagent2 = Agent(\n    agent_name="summarizer",\n    system_prompt="Sumamrize the blog post",\n    llm=llm,\n    max_loops=1,\n    dashboard=False,\n    tools=[],\n)\n\n# Create the Sequential workflow\nworkflow = SequentialWorkflow(\n    agents=[agent1, agent2], max_loops=1, verbose=False\n)\n\n# Run the workflow\nworkflow.run(\n    "Generate a blog post on how swarms of agents can help businesses grow."\n)\n\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import BaseLLM\n\nclass vLLMLM(BaseLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships. [Docs Available:](https://swarms.apac.ai/en/latest/swarms/structs/agent_rearrange/)\n\n```python\nfrom swarms import Agent, AgentRearrange, rearrange, Anthropic\n\n\n# Initialize the director agent\n\ndirector = Agent(\n    agent_name="Director",\n    system_prompt="Directs the tasks for the workers",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="director.json",\n)\n\n\n# Initialize worker 1\n\nworker1 = Agent(\n    agent_name="Worker1",\n    system_prompt="Generates a transcript for a youtube video on what swarms are",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="worker1.json",\n)\n\n\n# Initialize worker 2\nworker2 = Agent(\n    agent_name="Worker2",\n    system_prompt="Summarizes the transcript generated by Worker1",\n    llm=Anthropic(),\n    max_loops=1,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    state_save_file_type="json",\n    saved_state_path="worker2.json",\n)\n\n\n# Create a list of agents\nagents = [director, worker1, worker2]\n\n# Define the flow pattern\nflow = "Director -> Worker1 -> Worker2"\n\n# Using AgentRearrange class\nagent_system = AgentRearrange(agents=agents, flow=flow)\noutput = agent_system.run(\n    "Create a format to express and communicate swarms of llms in a structured manner for youtube"\n)\nprint(output)\n\n\n# Using rearrange function\noutput = rearrange(\n    agents,\n    flow,\n    "Create a format to express and communicate swarms of llms in a structured manner for youtube",\n)\n\nprint(output)\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tools\n├── utils\n└── workers\n```\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n## Accelerate Backlog\nAccelerate Bugs, Features, and Demos to implement by supporting us here:\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## Docker Instructions\n- [Learn More Here About Deployments In Docker]()\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
-    'author': 'Kye Gomez',
-    'author_email': 'kye@apac.ai',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kyegomez/swarms',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+<div align="center">
+
+Orchestrate swarms of agents for production-grade applications.
+
+[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)
+
+[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
+
+[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
+
+</div>
+
+
+Individual agents face 5 significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.
+----
+
+## Install
+`$ pip3 install -U swarms==4.9.7`
+
+---
+
+## Usage
+
+
+Run example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+### `Agent`
+A fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!
+
+Features:
+
+✅ Any LLM / Any framework
+
+✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc
+
+✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)
+
+```python
+import os
+
+from dotenv import load_dotenv
+
+# Import the OpenAIChat model and the Agent struct
+from swarms import Agent, OpenAIChat
+
+# Load the environment variables
+load_dotenv()
+
+# Get the API key from the environment
+api_key = os.environ.get("OPENAI_API_KEY")
+
+# Initialize the language model
+llm = OpenAIChat(
+    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000
+)
+
+
+## Initialize the workflow
+agent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)
+
+# Run the workflow on a task
+agent.run("Generate a 10,000 word blog on health and wellness.")
+```
+
+
+# `Agent` with Long Term Memory
+`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.
+
+```python
+from swarms import Agent, ChromaDB, OpenAIChat
+
+# Making an instance of the ChromaDB class
+memory = ChromaDB(
+    metric="cosine",
+    n_results=3,
+    output_dir="results",
+    docs_folder="docs",
+)
+
+# Initializing the agent with the Gemini instance and other parameters
+agent = Agent(
+    agent_name="Covid-19-Chat",
+    agent_description=(
+        "This agent provides information about COVID-19 symptoms."
+    ),
+    llm=OpenAIChat(),
+    max_loops="auto",
+    autosave=True,
+    verbose=True,
+    long_term_memory=memory,
+    stopping_condition="finish",
+)
+
+# Defining the task and image path
+task = ("What are the symptoms of COVID-19?",)
+
+# Running the agent with the specified task and image
+out = agent.run(task)
+print(out)
+
+```
+
+
+# `Agent` with Long Term Memory ++ Tools!
+An LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.
+
+```python
+from swarms import Agent, ChromaDB, OpenAIChat, tool
+
+# Making an instance of the ChromaDB class
+memory = ChromaDB(
+    metric="cosine",
+    n_results=3,
+    output_dir="results",
+    docs_folder="docs",
+)
+
+# Initialize a tool
+@tool
+def search_api(query: str):
+    # Add your logic here
+    return query
+
+# Initializing the agent with the Gemini instance and other parameters
+agent = Agent(
+    agent_name="Covid-19-Chat",
+    agent_description=(
+        "This agent provides information about COVID-19 symptoms."
+    ),
+    llm=OpenAIChat(),
+    max_loops="auto",
+    autosave=True,
+    verbose=True,
+    long_term_memory=memory,
+    stopping_condition="finish",
+    tools=[search_api],
+)
+
+# Defining the task and image path
+task = ("What are the symptoms of COVID-19?",)
+
+# Running the agent with the specified task and image
+out = agent.run(task)
+print(out)
+
+```
+
+### Simple Conversational Agent
+A Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models
+
+- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking
+- Reliable, this simple system will always provide responses you want.
+
+```python
+from swarms import Agent, Anthropic
+
+
+## Initialize the workflow
+agent = Agent(
+    agent_name="Transcript Generator",
+    agent_description=(
+        "Generate a transcript for a youtube video on what swarms"
+        " are!"
+    ),
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    interactive=True, # Set to True
+)
+
+# Run the workflow on a task
+agent("Generate a transcript for a youtube video on what swarms are!")
+```
+
+## Devin
+Implementation of Devil in less than 90 lines of code with several tools:
+terminal, browser, and edit files!
+
+```python
+from swarms import Agent, Anthropic, tool
+import subprocess
+
+# Model
+llm = Anthropic(
+    temperature=0.1,
+)
+
+# Tools
+@tool
+def terminal(
+    code: str,
+):
+    """
+    Run code in the terminal.
+
+    Args:
+        code (str): The code to run in the terminal.
+
+    Returns:
+        str: The output of the code.
+    """
+    out = subprocess.run(
+        code, shell=True, capture_output=True, text=True
+    ).stdout
+    return str(out)
+
+
+@tool
+def browser(query: str):
+    """
+    Search the query in the browser with the `browser` tool.
+
+    Args:
+        query (str): The query to search in the browser.
+
+    Returns:
+        str: The search results.
+    """
+    import webbrowser
+
+    url = f"https://www.google.com/search?q={query}"
+    webbrowser.open(url)
+    return f"Searching for {query} in the browser."
+
+@tool
+def create_file(file_path: str, content: str):
+    """
+    Create a file using the file editor tool.
+
+    Args:
+        file_path (str): The path to the file.
+        content (str): The content to write to the file.
+
+    Returns:
+        str: The result of the file creation operation.
+    """
+    with open(file_path, "w") as file:
+        file.write(content)
+    return f"File {file_path} created successfully."
+
+@tool
+def file_editor(file_path: str, mode: str, content: str):
+    """
+    Edit a file using the file editor tool.
+
+    Args:
+        file_path (str): The path to the file.
+        mode (str): The mode to open the file in.
+        content (str): The content to write to the file.
+
+    Returns:
+        str: The result of the file editing operation.
+    """
+    with open(file_path, mode) as file:
+        file.write(content)
+    return f"File {file_path} edited successfully."
+
+
+# Agent
+agent = Agent(
+    agent_name="Devin",
+    system_prompt=(
+        "Autonomous agent that can interact with humans and other"
+        " agents. Be Helpful and Kind. Use the tools provided to"
+        " assist the user. Return all code in markdown format."
+    ),
+    llm=llm,
+    max_loops="auto",
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    interactive=True,
+    tools=[terminal, browser, file_editor, create_file],
+    code_interpreter=True,
+    # streaming=True,
+)
+
+# Run the agent
+out = agent("Create a new file for a plan to take over the world.")
+print(out)
+```
+
+
+## `Agent`with Pydantic BaseModel as Output Type
+The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
+
+```python
+from pydantic import BaseModel, Field
+from swarms import Anthropic, Agent
+
+
+# Initialize the schema for the person's information
+class Schema(BaseModel):
+    name: str = Field(..., title="Name of the person")
+    agent: int = Field(..., title="Age of the person")
+    is_student: bool = Field(..., title="Whether the person is a student")
+    courses: list[str] = Field(
+        ..., title="List of courses the person is taking"
+    )
+
+
+# Convert the schema to a JSON string
+tool_schema = Schema(
+    name="Tool Name",
+    agent=1,
+    is_student=True,
+    courses=["Course1", "Course2"],
+)
+
+# Define the task to generate a person's information
+task = "Generate a person's information based on the following schema:"
+
+# Initialize the agent
+agent = Agent(
+    agent_name="Person Information Generator",
+    system_prompt=(
+        "Generate a person's information based on the following schema:"
+    ),
+    # Set the tool schema to the JSON string -- this is the key difference
+    tool_schema=tool_schema,
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    interactive=True,
+    # Set the output type to the tool schema which is a BaseModel
+    output_type=tool_schema,  # or dict, or str
+    metadata_output_type="json",
+    # List of schemas that the agent can handle
+    list_tool_schemas=[tool_schema],
+    function_calling_format_type="OpenAI",
+    function_calling_type="json",  # or soon yaml
+)
+
+# Run the agent to generate the person's information
+generated_data = agent.run(task)
+
+# Print the generated data
+print(f"Generated data: {generated_data}")
+
+
+```
+
+
+### `ToolAgent`
+ToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.
+
+
+```python
+from pydantic import BaseModel, Field
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+from swarms import ToolAgent
+from swarms.utils.json_utils import base_model_to_json
+
+# Load the pre-trained model and tokenizer
+model = AutoModelForCausalLM.from_pretrained(
+    "databricks/dolly-v2-12b",
+    load_in_4bit=True,
+    device_map="auto",
+)
+tokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")
+
+
+# Initialize the schema for the person's information
+class Schema(BaseModel):
+    name: str = Field(..., title="Name of the person")
+    agent: int = Field(..., title="Age of the person")
+    is_student: bool = Field(
+        ..., title="Whether the person is a student"
+    )
+    courses: list[str] = Field(
+        ..., title="List of courses the person is taking"
+    )
+
+
+# Convert the schema to a JSON string
+tool_schema = base_model_to_json(Schema)
+
+# Define the task to generate a person's information
+task = (
+    "Generate a person's information based on the following schema:"
+)
+
+# Create an instance of the ToolAgent class
+agent = ToolAgent(
+    name="dolly-function-agent",
+    description="Ana gent to create a child data",
+    model=model,
+    tokenizer=tokenizer,
+    json_schema=tool_schema,
+)
+
+# Run the agent to generate the person's information
+generated_data = agent.run(task)
+
+# Print the generated data
+print(f"Generated data: {generated_data}")
+
+```
+
+
+### `Worker`
+The `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.
+
+✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework
+
+✅ Reliable RAG: Utilizes FAISS for efficient RAG but it's modular so you can use any DB.
+
+✅ Multi-Step Parallel Function Calling: Use any tool
+
+```python
+# Importing necessary modules
+import os
+
+from dotenv import load_dotenv
+
+from swarms import OpenAIChat, Worker, tool
+
+# Loading environment variables from .env file
+load_dotenv()
+
+# Retrieving the OpenAI API key from environment variables
+api_key = os.getenv("OPENAI_API_KEY")
+
+
+# Create a tool
+@tool
+def search_api(query: str):
+    pass
+
+
+# Creating a Worker instance
+worker = Worker(
+    name="My Worker",
+    role="Worker",
+    human_in_the_loop=False,
+    tools=[search_api],
+    temperature=0.5,
+    llm=OpenAIChat(openai_api_key=api_key),
+)
+
+# Running the worker with a prompt
+out = worker.run("Hello, how are you? Create an image of how your are doing!")
+
+# Printing the output
+print(out)
+```
+
+------
+
+
+
+
+
+
+
+----
+
+### `SequentialWorkflow`
+Sequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.
+
+
+✅  Save and Restore Workflow states!
+
+✅  Multi-Modal Support for Visual Chaining
+
+✅  Utilizes Agent class
+
+```python
+from swarms import Agent, SequentialWorkflow, Anthropic
+
+
+# Initialize the language model agent (e.g., GPT-3)
+llm = Anthropic()
+
+# Initialize agents for individual tasks
+agent1 = Agent(
+    agent_name="Blog generator",
+    system_prompt="Generate a blog post like stephen king",
+    llm=llm,
+    max_loops=1,
+    dashboard=False,
+    tools=[],
+)
+agent2 = Agent(
+    agent_name="summarizer",
+    system_prompt="Sumamrize the blog post",
+    llm=llm,
+    max_loops=1,
+    dashboard=False,
+    tools=[],
+)
+
+# Create the Sequential workflow
+workflow = SequentialWorkflow(
+    agents=[agent1, agent2], max_loops=1, verbose=False
+)
+
+# Run the workflow
+workflow.run(
+    "Generate a blog post on how swarms of agents can help businesses grow."
+)
+
+```
+
+
+
+### `ConcurrentWorkflow`
+`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!
+
+
+```python
+import os
+
+from dotenv import load_dotenv
+
+from swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task
+
+# Load environment variables from .env file
+load_dotenv()
+
+# Load environment variables
+llm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))
+agent = Agent(llm=llm, max_loops=1)
+
+# Create a workflow
+workflow = ConcurrentWorkflow(max_workers=5)
+
+# Create tasks
+task1 = Task(agent, "What's the weather in miami")
+task2 = Task(agent, "What's the weather in new york")
+task3 = Task(agent, "What's the weather in london")
+
+# Add tasks to the workflow
+workflow.add(tasks=[task1, task2, task3])
+
+# Run the workflow
+workflow.run()
+```
+
+### `RecursiveWorkflow`
+`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!
+
+```python
+import os
+
+from dotenv import load_dotenv
+
+from swarms import Agent, OpenAIChat, RecursiveWorkflow, Task
+
+# Load environment variables from .env file
+load_dotenv()
+
+# Load environment variables
+llm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))
+agent = Agent(llm=llm, max_loops=1)
+
+# Create a workflow
+workflow = RecursiveWorkflow(stop_token="<DONE>")
+
+# Create tasks
+task1 = Task(agent, "What's the weather in miami")
+task2 = Task(agent, "What's the weather in new york")
+task3 = Task(agent, "What's the weather in london")
+
+# Add tasks to the workflow
+workflow.add(task1)
+workflow.add(task2)
+workflow.add(task3)
+
+# Run the workflow
+workflow.run()
+```
+
+
+
+### `SwarmNetwork`
+`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.
+
+✅ Efficient Task Management: SwarmNetwork's intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.
+
+✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.
+
+✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user's needs and infrastructure.
 
+```python
+import os
 
-setup(**setup_kwargs)
+from dotenv import load_dotenv
+
+# Import the OpenAIChat model and the Agent struct
+from swarms import Agent, OpenAIChat, SwarmNetwork
+
+# Load the environment variables
+load_dotenv()
+
+# Get the API key from the environment
+api_key = os.environ.get("OPENAI_API_KEY")
+
+# Initialize the language model
+llm = OpenAIChat(
+    temperature=0.5,
+    openai_api_key=api_key,
+)
+
+## Initialize the workflow
+agent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")
+agent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")
+agent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")
+
+
+# Load the swarmnet with the agents
+swarmnet = SwarmNetwork(
+    agents=[agent, agent2, agent3],
+)
+
+# List the agents in the swarm network
+out = swarmnet.list_agents()
+print(out)
+
+# Run the workflow on a task
+out = swarmnet.run_single_agent(
+    agent2.id, "Generate a 10,000 word blog on health and wellness."
+)
+print(out)
+
+
+# Run all the agents in the swarm network on a task
+out = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")
+print(out)
+```
+
+
+### `Task`
+`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation
+
+✅ Task is a structure for task execution with the Agent. 
+
+✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. 
+
+✅ The Task structure allows for efficient workflow automation with LLM-based agents.
+
+```python
+import os
+
+from dotenv import load_dotenv
+
+from swarms.structs import Agent, OpenAIChat, Task
+
+# Load the environment variables
+load_dotenv()
+
+
+# Define a function to be used as the action
+def my_action():
+    print("Action executed")
+
+
+# Define a function to be used as the condition
+def my_condition():
+    print("Condition checked")
+    return True
+
+
+# Create an agent
+agent = Agent(
+    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),
+    max_loops=1,
+    dashboard=False,
+)
+
+# Create a task
+task = Task(
+    description=(
+        "Generate a report on the top 3 biggest expenses for small"
+        " businesses and how businesses can save 20%"
+    ),
+    agent=agent,
+)
+
+# Set the action and condition
+task.set_action(my_action)
+task.set_condition(my_condition)
+
+# Execute the task
+print("Executing task...")
+task.run()
+
+# Check if the task is completed
+if task.is_completed():
+    print("Task completed")
+else:
+    print("Task not completed")
+
+# Output the result of the task
+print(f"Task result: {task.result}")
+```
+
+---
+
+
+
+
+## Majority Voting
+Multiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)
+
+```python
+from swarms import Agent, MajorityVoting, ChromaDB, Anthropic
+
+# Initialize the llm
+llm = Anthropic()
+
+# Agents
+agent1 = Agent(
+    llm = llm,
+    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",
+    agent_name="Progressive Leader",
+    agent_description="Leader of the Progressive Party",
+    long_term_memory=ChromaDB(),
+    max_steps=1,
+)
+
+agent2 = Agent(
+    llm=llm,
+    agent_name="Conservative Leader",
+    agent_description="Leader of the Conservative Party",
+    long_term_memory=ChromaDB(),
+    max_steps=1,
+)
+
+agent3 = Agent(
+    llm=llm,
+    agent_name="Libertarian Leader",
+    agent_description="Leader of the Libertarian Party",
+    long_term_memory=ChromaDB(),
+    max_steps=1,
+)
+
+# Initialize the majority voting
+mv = MajorityVoting(
+    agents=[agent1, agent2, agent3],
+    output_parser=llm.majority_voting,
+    autosave=False,
+    verbose=True,
+)
+
+
+# Start the majority voting
+mv.run("What is your stance on healthcare?")
+```
+
+## Real-World Deployment
+
+### Multi-Agent Swarm for Logistics
+Here's a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.
+
+
+```python
+import os
+
+from dotenv import load_dotenv
+
+from swarms.models import GPT4VisionAPI
+from swarms.prompts.logistics import (
+    Efficiency_Agent_Prompt,
+    Health_Security_Agent_Prompt,
+    Productivity_Agent_Prompt,
+    Quality_Control_Agent_Prompt,
+    Safety_Agent_Prompt,
+    Security_Agent_Prompt,
+    Sustainability_Agent_Prompt,
+)
+from swarms.structs import Agent
+
+# Load ENV
+load_dotenv()
+api_key = os.getenv("OPENAI_API_KEY")
+
+# GPT4VisionAPI
+llm = GPT4VisionAPI(openai_api_key=api_key)
+
+# Image for analysis
+factory_image = "factory_image1.jpg"
+
+# Initialize agents with respective prompts
+health_security_agent = Agent(
+    llm=llm,
+    sop=Health_Security_Agent_Prompt,
+    max_loops=1,
+    multi_modal=True,
+)
+
+# Quality control agent
+quality_control_agent = Agent(
+    llm=llm,
+    sop=Quality_Control_Agent_Prompt,
+    max_loops=1,
+    multi_modal=True,
+)
+
+
+# Productivity Agent
+productivity_agent = Agent(
+    llm=llm,
+    sop=Productivity_Agent_Prompt,
+    max_loops=1,
+    multi_modal=True,
+)
+
+# Initiailize safety agent
+safety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)
+
+# Init the security agent
+security_agent = Agent(
+    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True
+)
+
+
+# Initialize sustainability agent
+sustainability_agent = Agent(
+    llm=llm,
+    sop=Sustainability_Agent_Prompt,
+    max_loops=1,
+    multi_modal=True,
+)
+
+
+# Initialize efficincy agent
+efficiency_agent = Agent(
+    llm=llm,
+    sop=Efficiency_Agent_Prompt,
+    max_loops=1,
+    multi_modal=True,
+)
+
+# Run agents with respective tasks on the same image
+health_analysis = health_security_agent.run(
+    "Analyze the safety of this factory", factory_image
+)
+quality_analysis = quality_control_agent.run(
+    "Examine product quality in the factory", factory_image
+)
+productivity_analysis = productivity_agent.run(
+    "Evaluate factory productivity", factory_image
+)
+safety_analysis = safety_agent.run(
+    "Inspect the factory's adherence to safety standards",
+    factory_image,
+)
+security_analysis = security_agent.run(
+    "Assess the factory's security measures and systems",
+    factory_image,
+)
+sustainability_analysis = sustainability_agent.run(
+    "Examine the factory's sustainability practices", factory_image
+)
+efficiency_analysis = efficiency_agent.run(
+    "Analyze the efficiency of the factory's manufacturing process",
+    factory_image,
+)
+```
+---
+
+
+## `Multi Modal Autonomous Agents`
+Run the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.
+
+```python
+# Description: This is an example of how to use the Agent class to run a multi-modal workflow
+import os
+
+from dotenv import load_dotenv
+
+from swarms.models.gpt4_vision_api import GPT4VisionAPI
+from swarms.structs import Agent
+
+# Load the environment variables
+load_dotenv()
+
+# Get the API key from the environment
+api_key = os.environ.get("OPENAI_API_KEY")
+
+# Initialize the language model
+llm = GPT4VisionAPI(
+    openai_api_key=api_key,
+    max_tokens=500,
+)
+
+# Initialize the task
+task = (
+    "Analyze this image of an assembly line and identify any issues such as"
+    " misaligned parts, defects, or deviations from the standard assembly"
+    " process. IF there is anything unsafe in the image, explain why it is"
+    " unsafe and how it could be improved."
+)
+img = "assembly_line.jpg"
+
+## Initialize the workflow
+agent = Agent(
+    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True
+)
+
+# Run the workflow on a task
+agent.run(task=task, img=img)
+```
+----
+
+
+## Build your own LLMs, Agents, and Swarms!
+
+### Swarms Compliant Model Interface
+```python
+from swarms import BaseLLM
+
+class vLLMLM(BaseLLM):
+    def __init__(self, model_name='default_model', tensor_parallel_size=1, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.model_name = model_name
+        self.tensor_parallel_size = tensor_parallel_size
+        # Add any additional initialization here
+    
+    def run(self, task: str):
+        pass
+
+# Example
+model = vLLMLM("mistral")
+
+# Run the model
+out = model("Analyze these financial documents and summarize of them")
+print(out)
+
+```
+
+
+### Swarms Compliant Agent Interface
+
+```python
+from swarms import Agent
+
+
+class MyCustomAgent(Agent):
+
+    def __init__(self, *args, **kwargs):
+
+        super().__init__(*args, **kwargs)
+
+        # Custom initialization logic
+
+    def custom_method(self, *args, **kwargs):
+
+        # Implement custom logic here
+
+        pass
+
+    def run(self, task, *args, **kwargs):
+
+        # Customize the run method
+
+        response = super().run(task, *args, **kwargs)
+
+        # Additional custom logic
+
+        return response`
+
+# Model
+agent = MyCustomAgent()
+
+# Run the agent
+out = agent("Analyze and summarize these financial documents: ")
+print(out)
+
+```
+
+
+### Compliant Interface for Multi-Agent Collaboration
+
+```python
+from swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm
+
+
+# Build your own Swarm
+class MySwarm(BaseSwarm):
+    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.name = name
+
+    def run(self, task: str, *args, **kwargs):
+        # Add your multi-agent logic here
+        # agent 1
+        # agent 2
+        # agent 3
+        return "output of the swarm"
+
+
+# Add your custom swarm to the AutoSwarmRouter
+router = AutoSwarmRouter(
+    swarms=[MySwarm]
+)
+
+
+# Create an AutoSwarm instance
+autoswarm = AutoSwarm(
+    name="kyegomez/myswarm",
+    description="A simple API to build and run swarms",
+    verbose=True,
+    router=router,
+)
+
+
+# Run the AutoSwarm
+autoswarm.run("Analyze these financial data and give me a summary")
+
+
+```
+
+## `AgentRearrange`
+Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships. [Docs Available:](https://swarms.apac.ai/en/latest/swarms/structs/agent_rearrange/)
+
+```python
+from swarms import Agent, AgentRearrange, rearrange, Anthropic
+
+
+# Initialize the director agent
+
+director = Agent(
+    agent_name="Director",
+    system_prompt="Directs the tasks for the workers",
+    llm=Anthropic(),
+    max_loops=1,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    state_save_file_type="json",
+    saved_state_path="director.json",
+)
+
+
+# Initialize worker 1
+
+worker1 = Agent(
+    agent_name="Worker1",
+    system_prompt="Generates a transcript for a youtube video on what swarms are",
+    llm=Anthropic(),
+    max_loops=1,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    state_save_file_type="json",
+    saved_state_path="worker1.json",
+)
+
+
+# Initialize worker 2
+worker2 = Agent(
+    agent_name="Worker2",
+    system_prompt="Summarizes the transcript generated by Worker1",
+    llm=Anthropic(),
+    max_loops=1,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    state_save_file_type="json",
+    saved_state_path="worker2.json",
+)
+
+
+# Create a list of agents
+agents = [director, worker1, worker2]
+
+# Define the flow pattern
+flow = "Director -> Worker1 -> Worker2"
+
+# Using AgentRearrange class
+agent_system = AgentRearrange(agents=agents, flow=flow)
+output = agent_system.run(
+    "Create a format to express and communicate swarms of llms in a structured manner for youtube"
+)
+print(output)
+
+
+# Using rearrange function
+output = rearrange(
+    agents,
+    flow,
+    "Create a format to express and communicate swarms of llms in a structured manner for youtube",
+)
+
+print(output)
+
+```
+
+## `HierarhicalSwarm`
+Coming soon...
+
+
+---
+
+## Documentation
+Documentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)
+
+----
+
+## Folder Structure
+The swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs` that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.
+
+```sh
+├── __init__.py
+├── agents
+├── artifacts
+├── memory
+├── schemas
+├── models
+├── prompts
+├── structs
+├── telemetry
+├── tools
+├── utils
+└── workers
+```
+
+----
+
+## 🫶 Contributions:
+
+The easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)
+
+Swarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!
+
+<a href="https://github.com/kyegomez/swarms/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />
+</a>
+
+----
+
+## Community
+
+Join our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 
+
+- View our official [Blog](https://swarms.apac.ai)
+- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)
+- Follow us on [Twitter](https://twitter.com/kyegomez)
+- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)
+- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)
+- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)
+- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)
+
+---
+
+## Discovery Call
+Book a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)
+
+
+## Accelerate Backlog
+Accelerate Bugs, Features, and Demos to implement by supporting us here:
+
+<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>
+
+
+## Docker Instructions
+- [Learn More Here About Deployments In Docker](https://swarms.apac.ai/en/latest/docker_setup/)
+
+
+## Swarm Newsletter 🤖 🤖 🤖 📧 
+Sign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊
+
+[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)
+
+# License
+Apache License
+
+# Citation
+Please cite Swarms in your paper or your project if you found it beneficial in any way! Appreciate you.
+```bibtex
+@misc{swarms,
+  author = {Gomez, Kye},
+  title = {{Swarms: The Multi-Agent Collaboration Framework}},
+  howpublished = {\url{https://github.com/kyegomez/swarms}},
+  year = {2023},
+  note = {Accessed: Date}
+}
+```
```

