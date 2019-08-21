# iPay DEMO

სკრიპტი შექმნილია იმისათვის, რომ მაგალითზე ნახოთ როგორ შეიძლება ჩააშენოთ თქვენს საიტზე iPay საგადახდოს სისტემა და როგორ მუშაობს ის.

## მოთხოვნები

  - PHP 5 ან უფრო ახალი

## ინსტალაცია

ატვირთეთ ყველა ფაილი ვებ სერვერზე.

"index.php" ფაილში მერჩანტის იდენტიფიკატორში და საიდუმლო გასაღებში მითითებულია სატესტო მერჩანტის მონაცემები:

        $usernameAndPassword = '1006:581ba5eeadd657c8ccddc74c839bd3ad';

*პროდაქშენზე უნდა შეიცვალოს თქვენი მერჩანტის მონაცემებით 

დემო:

https://demo.ipay.ge/

## პროცესი

გადახდის პროცესი : //შესაცვლელია

- ყიდვა ღილაკზე დაჭერის შემდეგ კლიენტი გადის ავტორიზაციას iPay-ზე
- წარმატებული ვატორიზაციის შემდეგ სერვერი აბრუნებს ტოკენს და ტოკენის ტიპს
- კლიენტი ტოკენთან ერთად აგზავნის პროდუქტის დეტალებს
- სერვერი აბრუნებს ორ ლინკს:
    1. გადახდის სტატუსი და დეტალები
    2. iPay-ზე გადახდის გვერდზე გადასასვლელი ლინკი
- კლიენტი აკეთებს მომხმარებლის გადამისამართებას გადახდის გვერდზე სადაც არის გადახდის ორი მეთოდი:
    1. გადახდა ბარათით - გადახდა შესაძლებელია ნებისმიერი ბანკის ბარათით
    2. გადახდა ინტერნეტ ბანკით -  გადახდა სრულდება საქართველოს ბანკის ინტერნეტ ბანკის მომხმარებლით

დოკუმენტაციის სანახავად დააჭირეთ [აქ](https://ipay.ge/#dev)