## 12.01.2024
新知识：log_probs = torch.log_softmax(next_token_logits, dim=-1)，top_k_log_probs = torch.log_softmax(top_k_values, dim=-1).squeeze(0)，两种归一化的方法是不同的，前者是基于全局进行归一化，后者是基于topk进行归一化，固导致generate同样的token，prob不相同。
未完成：没有规整code并push，没有完成奇迹的创业表，没有把这两部分结合成一个方法，需要进一步提高效率。
已完成：完成基于dictionary作为constrain的beam search方法。完成计算accuracy的代码。




