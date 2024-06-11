# opps-assignment
class Product {
    name: string
    price: number

    constructor(n:string, p:number, ){this.name=n;
        this.price=p
    }

    display(){
        console.log(`${this.name}'s price is ${this.price}`)
    }
}

class Dress extends Product{
    name: string
    price:number
    sizeNo : string
    brand: string
    
    constructor(name:string,brand:string, price:number, sizeNo:string,){
        super(name,price)
        this.sizeNo = sizeNo
        this.brand = brand
        this.name = name
        this.price = price
    }
    Dresses(){
        super.display()
        console.log(`This shirt is from ${this.brand} and the size of this sweat shirt is ${this.sizeNo}`)
    }
}

let shirt = new Dress("Sweat shirt","adidas", 1000 , "Medium", )
shirt.Dresses()


class Fruit extends Product{
    name: string
    price:number
    colour: string
    expirydate: string
    
    constructor(name:string,expirydate:string, price:number, colour:string,){
        super(name,price)
        this.expirydate = expirydate
        this.name = name
        this.price = price
        this.colour = colour 
    }
    fruit(){
        super.display()
        console.log(`The colour Mango is ${this.colour} and expiry date of this Mango is ${this.expirydate}`)
    }
}

let fruit = new Fruit("Mango","12/10/2024", 250 , "yellow", )
fruit.fruit()

class Book extends Product{
    name: string
    price:number
    author: string
    
    constructor(name:string,author:string, price:number, ){
        super(name,price)
        this. price = price
        this.author = author
        this.name = name 
    }
    book(){
        super.display()
        console.log(`The author name is ${this.author}`)
    }
}

let book = new Book("Harry Potter","J. K. Rowling",500 )
book.book()
