# flutter_cicd_example

Flutter projesinde CICD sürecinin nasıl olduğunu inceleyelim.

## Getting Started

Öncelikle Projeyi Firebase App Distribution ile paylaşmak istiyorsak. Firebase bağlantılarını gerçekleştirmeliyiz.

Projemizin gizliliği için Reponun sağ üst tarafında bulunan settings butonuna tıklayıp: Settings > Secrets&Veriables > Actions > New Repository Secret adımlarını takip ederek gerekli FIREBASE_ID ve CREDENTIAL_FILE_CONTENT bilgilerini secrets olarak ekliyoruz.

![1](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/a6d50483-cf53-4897-80ed-c4b1276cd7a6)

![2](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/6045d868-36e2-473b-a6bd-a06dd21fe3c5)


Bu bilgilere nasıl ulaşacağımızı aşağıdaki görselleri takip ederek bulabilirsiniz.

![3](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/c45d03da-850f-487b-8fb2-31972f80fe18)

![4](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/48372ef7-4356-4d45-b265-8b6048eee126)

APP_ID Bilgisini bu şekilde aldık. Sırada CREDENTIAL_FILE_CONTENT bilgilerini almamız gerekiyor. Bunun için:

Öncelikle https://console.cloud.google.com linkine giriş yapmalıyız. Sonrasında bu adımları takip edeceğiz.

![5](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/c94c5ad9-b8a1-4449-a286-a1b078f0b950)

![6](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/88bee6ea-e057-4a40-8b0a-6f1245b41d55)

![7](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/c2f2ac8f-40b9-4bee-9690-05fef63f6bf2)

![8](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/297f3db1-8447-400f-aa41-ea552a394378)

![9](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/37f07b5a-2494-412f-a0af-71d300f0fbf9)

![10](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/1f845933-fcaa-4528-8b3f-c318c1a0983c)

![11](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/2f53e16f-6a2d-4fb9-acc8-4f36fcd2d717)

Artık CREDENTIAL_FILE_CONTENT bilgilerine sahip durumdayız. Şimdi tek yapmamız gereken kodu githubda main branchine pushlamamız ve Github-Actions sayesinde kodlarımız otomatik olarak derlenip Android Apk dosyasımız Firebase App Distribution'a yüklenecektir. 

![12](https://github.com/turedioglu/flutter-CICD-App-Distribution-For-Android/assets/32618134/c58e7ded-16f3-4fb7-8489-b60fd944a727)



