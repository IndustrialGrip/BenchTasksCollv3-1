# Final Pool - Implemented Tasks

This directory contains the tasks that are **verified as implemented** by developers in the BenchTasksCollv3 project, together with the tasks that are still being implemented.

## How a task was classified

A task is counted as `implemented` only when its directory on the developer branch satisfies the example task template in `tasks/examples/example-task`, i.e. it contains **all** of:

- `docs/agent_system_prompt.md`
- `docs/task.md`
- `docs/user_system_prompt.md`
- `evaluation/main.py`
- `preprocess/main.py`
- `initial_workspace/readme.txt`
- `groundtruth_workspace/readme.txt`

On top of that, the content requirements stated in the example task apply: `docs/task.md`, `docs/agent_system_prompt.md` and `docs/user_system_prompt.md` must be **non-empty and written entirely in English** (no Chinese).

Any task that is missing one of those files, or whose docs contain Chinese text, is counted as `implementing`.

(The template's own root `readme.txt` is not counted: no task directory under any developer branch contains one, so it is not part of the task contract.)

## Verified implemented tasks (5)

The files of these tasks are copied verbatim into `tasks/finalpool/<task_name>/`.

| Task | Implementor | Source on developer branch |
| --- | --- | --- |
| tag-manager | gyy | tasks/gyy/tag-manager |
| robots-handler | gyy | tasks/gyy/robots-handler |
| media-organizer | haoze | tasks/haoze/media-organizer |
| social-connector | junxian_dev | tasks/junxian/social-connector |
| client-portal | lueyang-dev | tasks/lueyang/client-portal |

## Verified implementing tasks (24)

These were added by the most recent task-adding commit on their developer branch, but they do **not** satisfy the requirements yet.

| Task | Implementor | Blocker |
| --- | --- | --- |
| discount-calculator | fan-dev | missing docs/user_system_prompt.md, initial_workspace/readme.txt, groundtruth_workspace/readme.txt |
| loyalty-program | fan-dev | missing preprocess/main.py, initial_workspace/readme.txt |
| sitemap-generator | gyy | missing evaluation/main.py |
| streaming-service | haoze | missing initial_workspace/readme.txt, preprocess/main.py |
| customer-feedback-processor | jl_dev | missing docs/user_system_prompt.md, preprocess/main.py |
| inventory-management | jl_dev | missing docs/user_system_prompt.md, initial_workspace/readme.txt, preprocess/main.py |
| customer-portal | junteng_dev | missing evaluation/main.py |
| help-desk | junteng_dev | missing initial_workspace/readme.txt |
| currency-converter | junxian_dev | docs/task.md contains a Chinese section, so it is not all English |
| territory-manager | lueyang-dev | missing initial_workspace/readme.txt, preprocess/main.py |
| analytics-dashboard | lv | missing groundtruth_workspace/readme.txt, initial_workspace/readme.txt, preprocess/main.py |
| insights-engine | lv | docs/agent_system_prompt.md contains a Chinese section, so it is not all English |
| survey-builder | lv | missing docs/user_system_prompt.md, groundtruth_workspace/readme.txt, preprocess/main.py |
| log-analyzer | ruige | missing docs/user_system_prompt.md, groundtruth_workspace/readme.txt |
| web-crawler | ruige | missing docs/user_system_prompt.md, groundtruth_workspace/readme.txt, preprocess/main.py |
| cache-optimizer | wenshuo-dev | missing docs/user_system_prompt.md, initial_workspace/readme.txt, groundtruth_workspace/readme.txt |
| scheduler | wenshuo-dev | missing groundtruth_workspace/readme.txt, preprocess/main.py |
| health-monitor | xiaochen_dev | missing docs/user_system_prompt.md |
| status-checker | xiaochen_dev | missing initial_workspace/readme.txt, groundtruth_workspace/readme.txt |
| sync-service | yuxuan-dev | missing groundtruth_workspace/readme.txt, preprocess/main.py |
| audit-logger | yuzhen-dev | docs/agent_system_prompt.md contains a Chinese section, so it is not all English |
| resource-monitor | yuzhen-dev | docs/agent_system_prompt.md contains a Chinese section, so it is not all English |
| certificate-manager | zhaochen | missing docs/user_system_prompt.md, initial_workspace/readme.txt, groundtruth_workspace/readme.txt, preprocess/main.py |
| storage-manager | zhaochen | missing docs/user_system_prompt.md, initial_workspace/readme.txt, groundtruth_workspace/readme.txt, preprocess/main.py |

## Source

The 29 tasks above come from the most recent task-adding commit on each developer branch of `toolathlon/BenchTasksCollv3`:

`fan-dev`, `gyy`, `haoze`, `jl_dev`, `junteng_dev`, `junxian_dev`, `lueyang-dev`, `lv`, `ruige`, `wenshuo-dev`, `xiaochen_dev`, `yuxuan-dev`, `yuzhen-dev`, `zhaochen`

(yuxuan-dev's commit message reads `Work on 2 tasks: sync-service,` with an empty second name, and only the `sync-service` directory was actually created.)

The same statuses are mirrored on the **Task Tracker** Notion page.
