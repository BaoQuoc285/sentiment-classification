## UIT_DS_NLI

Source pipeline code thi bảng B task Natural Language Interference. Nhóm tụi mình đã tách task NLI ra thành 2 phần là evidence retrieval và classification. Input sẽ là 1 đoạn văn bản và 1 câu premise đưa vaò evidence retrieval sẽ trả lại cho chúng ta 1 cặp premise và hypothesis rồi sau đó đưa cặp này vào phần classification để phân loại label.

Với evidence retrieval thì chúng mình dựa vào ensemble kết hợp nhiều pretrained model nhưng không tiến hành việc transfer learning.

Với classification tụi mình dùng pretrained model là xlm-roberta và tiến hành transfer learning trên đó để phân loại và trong file classification_train_inference ở dưới đã có phần cmt ở dưới là inference.
