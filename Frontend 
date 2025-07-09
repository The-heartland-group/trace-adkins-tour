import React, { useState } from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import {
  DropdownMenu,
  DropdownMenuTrigger,
  DropdownMenuContent,
  DropdownMenuItem,
} from "@/components/ui/dropdown-menu";

const tourDates = [
  { date: "Jul. 10, 2025", city: "Carlton, MN", venue: "Black Bear Casino Resort", price: 120, link: "https://gumroad.com/traceadkins-carlton" },
  { date: "Jul. 11, 2025", city: "La Vista, NE", venue: "The Astro Amphitheater", price: 150, link: "https://gumroad.com/traceadkins-lavista" },
  { date: "Jul. 12, 2025", city: "Troy, MO", venue: "Lincoln County Fair", price: 100, link: "https://gumroad.com/traceadkins-troy" },
  { date: "Jul. 25, 2025", city: "Hammondsport, NY", venue: "Point of the Bluff", price: 140, link: "https://gumroad.com/traceadkins-hammondsport" },
  { date: "Jul. 26, 2025", city: "Marietta, OH", venue: "Peoples Bank Theatre", price: 130, link: "https://gumroad.com/traceadkins-marietta" },
  { date: "Jul. 27, 2025", city: "Bay City, MI", venue: "Veterans Memorial Park", price: 120, link: "https://gumroad.com/traceadkins-baycity" },
  { date: "Aug. 1, 2025", city: "Ashland, KY", venue: "Paramount Arts Center", price: 160, link: "https://gumroad.com/traceadkins-ashland" },
  { date: "Aug. 2, 2025", city: "Columbus, OH", venue: "Ohio State Fair", price: 100, link: "https://gumroad.com/traceadkins-columbus" },
  { date: "Aug. 3, 2025", city: "Binghamton, NY", venue: "Spiedie Fest & Balloon Rally", price: 110, link: "https://gumroad.com/traceadkins-binghamton" },
  { date: "Aug. 8, 2025", city: "Welch, MN", venue: "Treasure Island Amphitheater", price: 200, link: "https://gumroad.com/traceadkins-welch" },
  { date: "Aug. 9, 2025", city: "Fort Dodge, IA", venue: "Central Plaza", price: 115, link: "https://gumroad.com/traceadkins-fortdodge" },
  { date: "Aug. 15, 2025", city: "Bristol, VA", venue: "Hard Rock Live", price: 180, link: "https://gumroad.com/traceadkins-bristol" },
  { date: "Aug. 16, 2025", city: "Elizabethtown, NC", venue: "Cape Fear Vineyard & Winery", price: 130, link: "https://gumroad.com/traceadkins-elizabethtown" },
  { date: "Aug. 17, 2025", city: "Lancaster, PA", venue: "American Music Theatre", price: 170, link: "https://gumroad.com/traceadkins-lancaster" },
  { date: "Aug. 21, 2025", city: "Princeton, IL", venue: "Bureau County Fair", price: 110, link: "https://gumroad.com/traceadkins-princeton" },
  { date: "Aug. 22, 2025", city: "Fort Wayne, IN", venue: "Foellinger Theatre", price: 140, link: "https://gumroad.com/traceadkins-fortwayne" },
  { date: "Aug. 23, 2025", city: "Spencer, IN", venue: "Tier 10 Music & Sports Park", price: 135, link: "https://gumroad.com/traceadkins-spencer" },
  { date: "Aug. 30, 2025", city: "Orland Park, IL", venue: "Centennial Park West", price: 125, link: "https://gumroad.com/traceadkins-orlandpark" },
  { date: "Sep. 1, 2025", city: "Wauseon, OH", venue: "Fulton County Fair", price: 100, link: "https://gumroad.com/traceadkins-wauseon" },
  { date: "Sep. 6, 2025", city: "Arcadia, FL", venue: "Mosaic Arena", price: 150, link: "https://gumroad.com/traceadkins-arcadia" },
  { date: "Sep. 13, 2025", city: "Fredericksburg, TX", venue: "The Resort at Fredericksburg", price: 160, link: "https://gumroad.com/traceadkins-fredericksburg" },
  { date: "Sep. 14, 2025", city: "Grand Prairie, TX", venue: "Texas Trust CU Theatre", price: 300, link: "https://gumroad.com/traceadkins-grandprairie" },
  { date: "Oct. 2, 2025", city: "Albuquerque, NM", venue: "Isleta Resort & Casino", price: 170, link: "https://gumroad.com/traceadkins-albuquerque" },
  { date: "Oct. 4, 2025", city: "Rancho Mirage, CA", venue: "Agua Caliente Resort Casino", price: 180, link: "https://gumroad.com/traceadkins-ranchomirage" },
  { date: "Oct. 5, 2025", city: "Cerritos, CA", venue: "Cerritos Center for the Performing Arts", price: 200, link: "https://gumroad.com/traceadkins-cerritos" },
  { date: "Oct. 10, 2025", city: "Fresno, CA", venue: "The Big Fresno Fair", price: 100, link: "https://gumroad.com/traceadkins-fresno" },
  { date: "Oct. 17, 2025", city: "Orange Park, FL", venue: "Thrasher-Horne Center", price: 160, link: "https://gumroad.com/traceadkins-orangepark" },
  { date: "Oct. 18, 2025", city: "Hiawassee, GA", venue: "Georgia Mountain Fairgrounds", price: 130, link: "https://gumroad.com/traceadkins-hiawassee" },
];

export default function TraceAdkinsTickets() {
  const [selectedShow, setSelectedShow] = useState(tourDates[0]);

  return (
    <div className="min-h-screen bg-gradient-to-b from-gray-900 to-black text-white p-6 flex flex-col items-center">
      <h1 className="text-4xl font-bold mb-4 text-center">🎸 Trace Adkins Official Tour 2025</h1>

      <Card className="bg-gray-800 border-gray-700 w-full max-w-xl">
        <CardContent className="p-6 space-y-4">
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button className="w-full bg-orange-600 hover:bg-orange-700" aria-label="Select a tour show">
                Select a Show: {selectedShow.city}
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent className="bg-gray-900 border-gray-700 text-white">
              {tourDates.map((show) => (
                <DropdownMenuItem
                  key={`${show.city}-${show.date}`}
                  onClick={() => setSelectedShow(show)}
                >
                  {show.city} – {show.date}
                </DropdownMenuItem>
              ))}
            </DropdownMenuContent>
          </DropdownMenu>

          <div className="bg-gray-900 p-4 rounded-xl border border-gray-700">
            <h2 className="text-xl font-semibold">{selectedShow.city}</h2>
            <p className="text-sm">📍 {selectedShow.venue}</p>
            <p className="text-sm">📅 {selectedShow.date}</p>
            <p className="text-sm">🕖 7:00 PM (Local Time)</p>
            <p className="text-sm">💵 ${selectedShow.price}</p>
            <p className="text-xs mt-2">
              🎫 After payment, you'll receive a confirmation email and QR code for entry.
            </p>
          </div>

          <a
            href={selectedShow.link}
            target="_blank"
            rel="noopener noreferrer"
          >
            <Button
              className="w-full bg-green-600 hover:bg-green-700 text-lg"
              aria-label={`Buy ticket for ${selectedShow.city} on ${selectedShow.date}`}
            >
              Buy Ticket
            </Button>
          </a>

          <div className="text-center text-xs text-gray-400">
            Prefer to pay with crypto? <br />
            DM us on Discord or visit{" "}
            <a
              href="https://nowpayments.io"
              target="_blank"
              rel="noopener noreferrer"
              className="underline text-blue-400"
            >
              NOWPayments
            </a>
          </div>
        </CardContent>
      </Card>
    </div>
  );
}