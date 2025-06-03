import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Input } from "@/components/ui/input"; import { Textarea } from "@/components/ui/textarea"; import { Mail, Phone, Calendar, DollarSign } from "lucide-react";

export default function BelovedSonWebsite() { return ( <div className="max-w-5xl mx-auto sm:p-4 p-6 space-y-10"> <section className="text-center space-y-4"> <h1 className="text-3xl sm:text-4xl font-bold">Beloved Son</h1> <p className="text-lg text-gray-700"> Sharing lived experiences with HIV, incarceration, and mental health to inspire healing and social change. </p> <Button className="mt-2">Download Mission Book</Button> </section>

<section className="grid grid-cols-1 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
    <Card>
      <CardContent className="space-y-2 p-4 text-center">
        <Calendar className="mx-auto text-blue-500" size={32} />
        <h3 className="text-xl font-semibold">Book My Services</h3>
        <p>Invite Beloved Son to speak, consult, or lead workshops.</p>
        <Button className="w-full" asChild>
          <a
            href="https://calendly.com/bigbrotherbeloved-ibg/coaching-ministry-of-presence"
            target="_blank"
            rel="noopener noreferrer"
          >
            Book Now
          </a>
        </Button>
      </CardContent>
    </Card>

    <Card>
      <CardContent className="space-y-2 p-4 text-center">
        <Mail className="mx-auto text-green-500" size={32} />
        <h3 className="text-xl font-semibold">Contact Me</h3>
        <p>Reach out for collaborations, press, or questions.</p>
        <form action="https://formspree.io/f/your-form-id" method="POST" className="space-y-2">
          <Input placeholder="Your email" type="email" name="email" required />
          <Textarea placeholder="Your message" name="message" required />
          <Button className="w-full" type="submit">Send</Button>
        </form>
      </CardContent>
    </Card>

    <Card>
      <CardContent className="space-y-2 p-4 text-center">
        <DollarSign className="mx-auto text-yellow-500" size={32} />
        <h3 className="text-xl font-semibold">Support the Mission</h3>
        <p>Your donation helps spread this vital message.</p>
        <Button className="w-full" asChild>
          <a
            href="https://ko-fi.com/belovedson"
            target="_blank"
            rel="noopener noreferrer"
          >
            Donate
          </a>
        </Button>
      </CardContent>
    </Card>
  </section>
</div>

); }

