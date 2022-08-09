# hw-2-lists
package com.example.hw_2_lists

fun main() {

    // Read-only (immutable)
    val names = listOf("Ahad", "Turki", "Raghad", "Nasser", "Sumayah", "Fahdah")
    val namesAll = listOf("Ahad", "Turki", "Raghad", "Nasser")
    val color = listOf<String>()

    // Read and Write (mutable)
    val numbers = mutableListOf("one", "two", "three", "four", "five")
    val weekDays = mutableListOf("Sun", "Mon", "Tue", "Wed", "Thurs", "Fri", "Sat")


    // Read-Write (mutable) List - Operations
    println("\n------- Read-Write (mutable) List - Operations -------\n")

    // Add (Element)
    println("\n----------- Add (Element) -----------\n")
    println("Befor add : ${numbers}")
    numbers.add("six")
    println("After add : ${numbers}")

    // Add (Index, Element)
    println("\n----------- Add (Index, Element) -----------\n")
    println("Befor add : ${numbers}")
    numbers.add(5,"seven")
    println("After add : ${numbers}")

    // Add All (List)
    println("\n----------- Add All (List) -----------\n")
    println("Befor add all : ${numbers}")
    numbers.addAll(weekDays)
    println("After add all : ${numbers}")
    // Add All (Index, List)
    println("\n----------- Add All (Index, List) -----------\n")

    println("Befor add all : ${numbers}")
    numbers.addAll(0,weekDays)
    println("After add all : ${numbers}")

    // Clear
    val number = mutableListOf(1,2,3,4,5)
    println("\n----------- Clear -----------\n")
    println("Befor use clear : ${number}")
    number.clear()
    println("After use clear : ${number}")
    // Remove
    println("\n-------------- Remove -------------\n")
    println("Befor remove one : ${numbers}")
    numbers.remove("one")
    println("After remove one : ${numbers}")
    // Remove At
    println("\n------------- Remove At -----------\n")
    println("Befor remove at : ${numbers}")
    numbers.removeAt(0)
    println("After remove at : ${numbers}")
    // Remove All
    println("\n----------- Remove All -----------\n")
    println("Befor remove all : ${numbers}")
    numbers.removeAll(weekDays)
    println("After remove all : ${numbers}")

    // Read-only (immutable) List - Operations
    println("\n----------- Read-only (immutable) List - Operations -----------\n")
    // The size of the list
    println("The size of the list numbers : ${ numbers.size } ")

    // Contains
    println("\n----------- Contains -----------\n")
    println("contains khloud : ${names.contains("khloud")}")
    println("contains Turki : ${names.contains("Turki")}")

    // Contains All
    println("\n----------- Contains All -----------\n")
    println(" ${names.containsAll(namesAll)}")

    // get
    println("\n----------- get -----------\n")
    println(" ${names.get(1)}")
    // indexOf
    println("\n----------- indexOf -----------\n")
    println(" ${names.indexOf("Ahad")}")
    // isEmpty
    println("\n----------- isEmpty -----------\n")
    println(" ${names.isEmpty()}")
    println(" ${color.isEmpty()}")
    // Sublist
    println("\n----------- Sublist -----------\n")
    println("Befor subList : ${names}")
    println("After subList : ${names.subList(2,5)}")

}
