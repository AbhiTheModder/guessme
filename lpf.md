 How Lucky Patcher works on some flutter apps.
----------------------------------------------

#### Some of you have either in the past or present surely have thought about how lucky patcher is able to manipulate aps written in dart (i.e., basically a form of C like programming language) which packages the Dart code inside lib during generating output for android releases...

**Author:** _[AbhiTheModder](https://guessme.pages.dev)_

#### The Answer:

Answer to this question is pretty simple if you look into the [FlutterInappPurchase.](https://pub.dev/packages/in_app_purchase) packages of flutter.

  

**Pros:**

 It has features of providing billing Api to flutter apps and without google play Api binding i.e., you don't need to use traditional way of adding play billing-api, services-api inside your _build.gradle_ anymore...Instead of that just use this flutter package and you're good to go.

[![](https://blogger.googleusercontent.com/img/a/AVvXsEifXPUM7f0J1syHaK5CCt5yGjTAlOqor9iXJr-LEeipG-wE7_lEelvgmkj0UeGTkF5iRddwfss6WXgN2ySErdezpvqZrod2gg3ym0AzOAJyzsqQWaTv_qnkbifWUN0BaM8IzXU6oU7C80mDVaeHHAJZLUyaokFTuu_qbF0BtvKw0ZMOUoBms3aaDIr_q-g=w640-h418)](https://blogger.googleusercontent.com/img/a/AVvXsEifXPUM7f0J1syHaK5CCt5yGjTAlOqor9iXJr-LEeipG-wE7_lEelvgmkj0UeGTkF5iRddwfss6WXgN2ySErdezpvqZrod2gg3ym0AzOAJyzsqQWaTv_qnkbifWUN0BaM8IzXU6oU7C80mDVaeHHAJZLUyaokFTuu_qbF0BtvKw0ZMOUoBms3aaDIr_q-g)

Source: [in\_app\_purchase](https://pub.dev/packages/in_app_purchase)

  
  

  

**Cons:**

The feature of this package that allows you to implement purchases through any store app you want to inside your build.

[![](https://blogger.googleusercontent.com/img/a/AVvXsEijOh9HXMVS0d7byRk_DAf7nNtbH9J8j_sGT04HhzgnTRILb_0G9NbYjEnFIHkJ2yoU1Z8tFfkH1MSdgf24PFHDKvDrekzcjuwfViZe4wItyekQ8HNNGbEtkVtid43iZCUEMck7Htaf-GTclzHmfrE1nQNvwwd5Z3aubYj7zbkNFf7t2A9e6SqKu519fec=w640-h164)](https://blogger.googleusercontent.com/img/a/AVvXsEijOh9HXMVS0d7byRk_DAf7nNtbH9J8j_sGT04HhzgnTRILb_0G9NbYjEnFIHkJ2yoU1Z8tFfkH1MSdgf24PFHDKvDrekzcjuwfViZe4wItyekQ8HNNGbEtkVtid43iZCUEMck7Htaf-GTclzHmfrE1nQNvwwd5Z3aubYj7zbkNFf7t2A9e6SqKu519fec)

Source: [in\_app\_purchase](https://pub.dev/packages/in_app_purchase)

If you read the highlighted line in the above picture, you'll understand that this package gives you ability to _**pass purchases to any store app**_ in your device, that means the developer can add feature for stores like **Mi store**,palm store,Vivo store apps comes with devices.

  

**Example dump.dart from such an app:**

[![](https://blogger.googleusercontent.com/img/a/AVvXsEhwRcUplhe2CUloKD6_E8Kl3rDdNT9asWPWdbHbBZZFr0unHhhTBu6tDGw_cz3AGMhJ-tm1cfzdLAR5jtMXPNrsyfXh25VaHvsrRJGi21LT5AItSzKT6Ew64PmIgoGL-oG2cs_dZY7lH6kS1YDZPl5pM8brPfmIClSP4nAp9u72wzQYFaL_jJDRRM5UlbY=w482-h288)](https://blogger.googleusercontent.com/img/a/AVvXsEhwRcUplhe2CUloKD6_E8Kl3rDdNT9asWPWdbHbBZZFr0unHhhTBu6tDGw_cz3AGMhJ-tm1cfzdLAR5jtMXPNrsyfXh25VaHvsrRJGi21LT5AItSzKT6Ew64PmIgoGL-oG2cs_dZY7lH6kS1YDZPl5pM8brPfmIClSP4nAp9u72wzQYFaL_jJDRRM5UlbY)

dumped using reFlutter

  

This is where we get **answer** to our main question "_How LP works on these apps?_":

As we get to know this package applied feature through which user can get purchasing from any store app present in your device.... and we also know what LP does is doing same applying it's patches inside app and showing it that it is systems store app and LP bypasses it as this package also in the same way stores the data received from store app and saves your purchases... LoL 🤣

[![](https://blogger.googleusercontent.com/img/a/AVvXsEjFLsC7WYZuk8AZ3ICyBs_JQXu2jHzuRm-A9ISZMTxtl4xBoMUCDdHaQsP8c9YMUDtp9PzXsUihHyPptRzBXNM8lTg1F-kZjRJuP5Z8gPBhPLiq5GWo5aFkdSRA6mTpXR99eSeBdXDyfw23HYArbD9q_4otLFyC4aM_eh6c5N-cfT3uqYj_AonXutY8m_I=w640-h214)](https://blogger.googleusercontent.com/img/a/AVvXsEjFLsC7WYZuk8AZ3ICyBs_JQXu2jHzuRm-A9ISZMTxtl4xBoMUCDdHaQsP8c9YMUDtp9PzXsUihHyPptRzBXNM8lTg1F-kZjRJuP5Z8gPBhPLiq5GWo5aFkdSRA6mTpXR99eSeBdXDyfw23HYArbD9q_4otLFyC4aM_eh6c5N-cfT3uqYj_AonXutY8m_I)

Source: [in\_app\_purchase](https://pub.dev/packages/in_app_purchase)

  
The above image clarify that it _validates your purchase through store app_ and then saves and you're done 😂
