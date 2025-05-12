# keystone-leads-site
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

export default function Home() {
  return (
    <div className="min-h-screen bg-gray-50 text-gray-900">
      <header className="bg-white shadow p-6 flex justify-between items-center">
        <h1 className="text-2xl font-bold">Keystone Leads</h1>
        <Button className="rounded-2xl px-6" size="lg">Book a Call</Button>
      </header>

      <main className="px-6 py-12 max-w-5xl mx-auto">
        {/* Hero Section */}
        <section className="text-center mb-16">
          <h2 className="text-4xl font-bold mb-4">Get 5–15 Exclusive Remodel Leads Every Month</h2>
          <p className="text-xl mb-6">We help kitchen & bath remodelers land $30k+ projects predictably — with premium homeowner leads, not tire-kickers.</p>
          <Button className="rounded-2xl px-8 text-lg" size="lg">Book Your Strategy Call</Button>
        </section>

        {/* How it Works */}
        <section className="mb-16">
          <h3 className="text-3xl font-semibold mb-6">How It Works</h3>
          <div className="grid md:grid-cols-3 gap-6">
            {["Target High-End Homeowners", "Deliver Exclusive Leads", "You Close $30k+ Projects"].map((step, i) => (
              <Card key={i} className="p-4 text-center">
                <CardContent>
                  <h4 className="text-xl font-bold mb-2">Step {i + 1}</h4>
                  <p>{step}</p>
                </CardContent>
              </Card>
            ))}
          </div>
        </section>

        {/* Results Section */}
        <section className="mb-16">
          <h3 className="text-3xl font-semibold mb-6">Results You Can Expect</h3>
          <ul className="space-y-4 text-lg">
            <li>✓ 15+ exclusive kitchen remodel leads in 90 days</li>
            <li>✓ $100k+ in new project pipeline within 6 months</li>
            <li>✓ 3–5 new $30k+ projects/month</li>
          </ul>
        </section>

        {/* Guarantee */}
        <section className="mb-16 bg-white p-6 rounded-2xl shadow">
          <h3 className="text-3xl font-semibold mb-4">Our Guarantee</h3>
          <p className="text-lg">If we don’t deliver 15 qualified homeowner leads in 90 days — you don’t pay. Simple as that.</p>
        </section>

        {/* About Section */}
        <section className="mb-16">
          <h3 className="text-3xl font-semibold mb-6">Why Remodelers Choose Us</h3>
          <ul className="space-y-4 text-lg">
            <li>✓ We specialize ONLY in high-end remodeling leads</li>
            <li>✓ Our leads are exclusive (never shared)</li>
            <li>✓ We’ve helped remodelers close $100k+ projects reliably</li>
          </ul>
        </section>

        {/* CTA Banner */}
        <section className="bg-gray-100 p-8 rounded-2xl text-center">
          <h3 className="text-2xl font-bold mb-4">Ready to Book More $30k+ Projects?</h3>
          <Button className="rounded-2xl px-8 text-lg" size="lg">Book Your Call Now</Button>
        </section>
      </main>

      <footer className="text-center p-6 text-sm text-gray-500">
        © 2025 Keystone Leads. All rights reserved.
      </footer>
    </div>
  );
}
