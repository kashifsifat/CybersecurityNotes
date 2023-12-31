### প্রসংগ : সাইবার সিকিউরিটি

#### পাবলিক কি ক্রিপ্টোগ্রাফি

আচ্ছা ধরেন, আমি আপনাকে মেসেজ করবো -

"HOW ARE YOU"

এখন যদি আমি এই মেসেজের প্রতিটা লেটার পরবর্তী তৃতীয় লেটার দিয়ে শিফট/রিপ্লেস করি,
তাইলে মেসেজ টা দাঁড়াবে -

"KRZ DUH BRX"

এখন ধরেন, অন্য কোনো মানুষ নয়, শুধু আমি আর আপনি জানি যে, আমরা প্রতিটা লেটার তার 'পরবর্তী' তৃতীয় লেটার দিয়ে রিপ্লেস করছি।

এখন, আপনার কাছে যখন এই মেসেজটা পাঠাবো, KRZ DUH BRX তখন আপনি এটার প্রতিটা লেটার কে তার 'পূর্ববর্তী' তৃতীয় লেটার দিয়ে রিপ্লেস করলেই আসল মেসেজটা জানতে পারবেন।

আর এই গোপন কোড টা হলো Encrypted মেসেজ।
আর নরমাল লিখাটা হলো Decrypted মেসেজ।

এখন এটা হলো জাস্ট Encryption - Decryption কেজি লেভেলের বিষয়।

এটারই অনেক অনেক এডভান্সড লেভেলের ইউজ হয় সাইবার সিকিউরিটিতে।

এখন যে প্রতিবারই থার্ড লেটার হবে এমন কোনো কথা নাই। ফোর্থ হতে পারে। ফিফথ হতে পারে। টেন্থ হতে পারে...

তো এখন যেই সিস্টেমের কথা বললাম এটাকে বলে Symmetric Key Encryption.
কিন্তু এই সিস্টেমটার একটা সমস্যা আছে।
আর তা হলো Key Sharing.

এই যে কোনো একটা মেসেজকে ৩, ৪, ১০, ১২ কতো তম লেটার দ্বারা রিপ্লেস করা হবে, সেটাই হলো Key.

এখন সমস্যা হলো গিয়ে, আমি যদি আপনার সাথে Symmetric Encryption ইউজ করি, তাহলে আমার অবশ্যই আপনাকে Key টা জানাতে হবে।

এর ভয়াবহ দিক হলো, যখন আমি আপনাকে Key টা জানাবো (Cybercesurity এর ভাষায় যাকে বলে 'Key Sharing') তখন এই Shared Key টা কোনোক্রমে ফাস হয়ে গেলে পুরা সিকিউরিটিই বরবাদ হয়ে যাবে।

ধরেন, কেউ জেনে গেলো, যে আমাদের Key = 4. অর্থাৎ, আমরা প্রতিটা লেটার কে পরবর্তী ৪ নাম্বার লেটার দ্বারা রিল্পেস করছি।

তাহলে কী হবে?

এখন আমরা যা-ই মেসেজ পাঠাই না কেনো, সেই দুষ্টলোক জেনে যাবে (যেহেতু সে Key টা জেনে গেছে)।

এটুকু বুঝেছেন আশা করি। এবার আসেন একটু অন্য দিকে ঘুরে আসি।

আচ্ছা, এক ধরনের তালা পাওয়া যায় যে জানেন নিশ্চই - যেগুলি লক খুলতে এবং লক করতে - দু'ক্ষেত্রেই চাবি লাগে। মানে চাবি ঘুরিয়েই লক করে, আর চাবি ঘুরিয়েই ওপেন করে।

তো, Symmetric Encryption এর এই Key চুরির সমস্যা ঠেকাতে Asymmetric Encryption উদ্ভাবন করা হয়েছে।

চলেন সহজে বুঝাই।

ধরেন, এমন একটা তালা আছে। যেটা আমরা চাবি দিয়ে লক করি। আবার চাবি দিয়েই আনলক করি।

এখন ধরেন, আমাদের ক্লাসরুমের এমন একটা লক আছে।

চাবি দিয়ে লক-আনলক করার।

কিন্তু, কেমন হবে বলেনতো, যদি দুইটাই এক রকম চাবি না হয়ে দুইটা দু'রকম হয়?

একটা দিয়ে লক করে, আর অন্যটা দিয়ে আনলক!

ধরেন, আমাদের ক্লাস শেষে রুমে আড্ডা দিচ্ছি।
স্যার তালাটা দিয়ে বললেন তোমরা যাওয়ার সময় লক করে দিও - তোমাদের যে কারো কাছে থাকা - এই তালা লক করার চাবি দিয়ে।

আর আনলক করার চাবি অনলি স্যারের কাছে আছে।

এখন কী হবে বিষয়টা?

আমরা আড্ডা শেষে সেই তালা লক করার চাবি দিয়ে তালা লক করে চলে আসবো।

কিন্তু, আনলক করার চাবি যেহেতু শুধুমাত্র স্যারের কাছে, তাই শুধুমাত্র স্যার তার কাছ থাকা চাবি দিয়ে পরদিন তালাটা খুলতে পারবেন।

এতোটুকু ক্লিয়ার?

এই হলো, Asymmetric Key Encryption.

এখানে প্রত্যেকের একটা লকিং আর একটা আনলকিং চাবি থাকে।

লক করারা চাবিটার কপি সবার কাছে পাবলিকলি শেয়ার করা হয়।
যাতে করে যে কোনো মেসেজ সেন্ডার লক করে (অর্থাৎ Encrypt করে) মেসেজ পাঠাতে পারে।
আর এই Key যেহেতু পাবলিকলি শেয়ার করা হয় তাই একে Public Key বলে।

আর আনলক করার চাবি শুধুমাত্র মেসেজ রিসিভার এর কাছেই থাকে। কক্ষনোই শেয়ার করা হয় না।
আর এই আনলক করার চাবিটা দিয়ে রিসিভার তার কাছে লক করে পাঠানো মেসেজ আনলক করে (অর্থাৎ Decrypt করে)।
আর এই Key যেহেতু কক্ষনোই শেয়ার করা হয় না, বরং সর্বাবস্থায় Private থাকে, তাই একে বলে Private Key.

এখন ধরেন আপনি আমাকে একটা Encrypted মেসেজ পাঠাবেন।
এখন আপনার দরকার হবে, আমার Public Key.

আপনি যখন আমার Public Key দিয়ে Encrypted মেসেজ আমাকে পাঠাবেন, তখন আমি আমার Private Key দিয়ে সেটা Decrypt করবো।

আবার বিপরীতভাবে,

ধরেন আমি আপনাকে একটা Encrypted মেসেজ পাঠাবো।
তখন আমার দরকার হবে আপনার Public Key.

আমি যখন আপনার Public Key দিয়ে Encrypted মেসেজ আপনাকে পাঠাবো, তখন আপনি আপনার Private Key দিয়ে সেটা Decrypt করবেন।

এটুকু বুঝেছেন?

আরেকটা জিনিস হলো,
মেসেজ এনক্রিপশন আবার দুই ধরনের হয়।

একটা হলো End-to-End.
অর্থাৎ, সোজা ইউজার থেকে ইউজার।
এক্ষেত্রে মাঝখানে সার্ভিস প্রোভাইডারও মেসেজটা জানতে পারে না।
তাই এটাকে বলা হয়, Zero-knowledge Encryption (যেহেতু সার্ভিস প্রোভাইডারও Decryption Key জানে না)।

আর অন্যটা হলো Clien - Server - Client.
এক্ষেত্রে, মেসেজটা সেন্ডার থেকে সার্ভিস প্রোভাইডার পর্যন্ত এনক্রিপ্টেড থাকে। তারপর সার্ভিস প্রোভাইডারের সার্ভারে গিয়ে মেসেজটা ডিক্রিপ্টেড হয়। তারপর সার্ভার থেকে আবার এনক্রিপ্ট করে মেসেজটা রিসিভারকে পাঠানো হয়।
এটা কম্পারেটিভলি ইনসিকিউরড।

আর কোন সার্ভিস কেমন সিকিউরড তা জানার ওয়ে বলতে গেলে, তা তাদের Privacy Policy-তেই প্রায়ই লিখা থাকে।

কিন্তু, আমরা বাংগালিরা তো শুধু শর্টকাট খুঁজি, তাই কখনোই Privacy Policy পড়ি না।

জাস্ট, next, next, next মেরে install করেই ইউজ করা শুরু করে দেই।

তো, এই ব্যাপারে একটু সতর্ক হলেই হয় আরকি।

আর Wikipedia থেকেও সেই সার্ভিস এর History, Privacy আর Security অংশটা পড়লে অনেক কিছুই জানা যায় ইজিলি।

আর ইন্টারনেট তো আছেই...
