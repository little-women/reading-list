```mermaid
        gantt
        dateFormat  YYYY-MM-DD
        title 周计划-Wei

        section 调研
        Paper-CCM                      :done, paper1, 2019-04-11,1d
        Paper-DSTC7                    :done, paper2, after paper1, 1d
        Paper-MemNet                   :done, paper3, after paper2, 1d
        
        section 开发
        Code-CCM                      :crit, active, 2019-04-11,2d
        Code-MemNet                   :after paper2, 2d
    
        section 测试
        调参，试使用预训练的embedding       :crit, after paper1, 36h
        尝试参照 CCM 改进                   :after paper2, 2d
```

```mermaid
        gantt
        dateFormat  YYYY-MM-DD
        title 周计划-Wei
        
        section 学习
        Paper-DAWnet      :active, 2019-04-16, 1d
        TransE 学习          :crit, active, study1, 2019-04-16, 1d
        预训练模型的使用          :after study1, 36h
        
        section 开发
        Code-CCM                      :crit, active,2019-04-15, 1d
        Code-MemNet                   :crit, active,2019-04-15, 1d
        调参，试使用预训练的embedding       :crit, active,2019-04-16, 2d
    
        section 测试
        尝试参照 CCM 改进                   :crit, active, task1, 2019-04-16, 2d
        调参                        :task2, after task1, 2d
```

