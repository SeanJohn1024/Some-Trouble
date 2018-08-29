# Some-Trouble

//IOS8中删除最后一个cell的时，报一个错误 

[RemindersCell _setDeleteAnimationInProgress:]: message sent to deallocated instance



重新刷新tableView的时候延迟一下

dispatch_after(dispatch_time(DISPATCH_TIME_NOW, (int64_t)(0.2 * NSEC_PER_SEC)), dispatch_get_main_queue(), ^{

                 [self.tableView reloadData];

            });
