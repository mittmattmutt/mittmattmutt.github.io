# Philosophy Of Language in 9 Sentences

I was recently reading something on Newtonian mechanics and was impressed by how
much information about the world could be presented so concisely: in three laws
by Newton, and in several pages in the pop science book I was reading. I got to
thinking whether the same could be done for my field, analytic philosophy of
language, and the below is the result.

There’s a lot of material here. It would be optimistic to think I’ve described
it all suitably well that someone without background could understand it all.
But I hope even if some of the details elude you, the style of argument, the
sort of theoretical considerations, and the basic shape of the discipline will
be clear to you if you give this article the fifteen minutes medium estimates
it’ll take to read.

#### Foundations

Let’s introduce some ideas that will stick with us as the foundations of our
theory of language, and before presenting 9 sentences which challenge those
foundations, and the changes that have been made in response to them. At the
heart of the philosophy of language is the truism that we use language to
describe objects. Objects are a certain way, have certain properties, and that’s
what we talk about. To do so, we have words which talk about objects (such as
names and pronouns like ‘this’ or ‘she’) and words which describe them (such as
verbs and adjectives and adjectival phrases like ‘runs’ and ‘tall’ and ‘is a
cat’).

One way to cash this out is by means of *referential semantics*. We say that
names(\pronouns) refer to objects, and that verbs(\adjectives\adjectival
phrases) refer to sets of objects, namely the set of objects the verb (\etc.)
correctly describes (‘run[s]’ refers to the set of things which run). We can
then say that a sentence like ‘Obama runs’ is true provided the object is a
member of the set referred to by the verb, that is provided Obama is a member of
the set of running things.

We can then add a layer of fanciness. Consider ‘it’s not the case that Obama
runs’. If we could view ‘Obama runs’ as referring to an object, then we could
treat ‘it’s not the case that’ as kind of like a verb(\etc.) in that it
describes an object. But what sort of object does ‘Obama runs’ stand for?

Well, we know this: a sentence is true or false. Moreover, at least for the case
we’re considering, that seems to be the *only* relevant thing about it: if we
know merely whether or not a sentence s is true or false, we also immediately
know whether ‘it’s not the case that s’ is true or false.

So maybe we could say this: a sentence refers to its truth value, which is a
weird new sort of object out there in the world. So ‘grass is green’ refers to
True, and ‘grass is black’ refers to False. We could then say that ‘it’s not the
case that’ refers to the set of sentences refer to False. We can say the same
thing with ‘and’ and ‘or’: they describe pairs of sentences, just as ‘loves’
describes pairs of objects.

That already gets us quite far. Having spelled out the details about how
transitive verbs like ‘loves’ works we will be able to give a referential
semantics for all sentences of the form: ‘Obama runs’, ‘Obama doesn’t run’,
‘Obama loves Michelle’, ‘Obama runs and Michelle doesn’t dance or Malia sings’,
and so on.

We’re going to take this model and run with it, by considering how in the course
of the 20th century it has been modified and improved to deal with ever greater
parts of natural languages.

### **9 Tricky Sentences**

#### 1. Everybody loves somebody (Frege, Begriffsschrift)

Surprisingly, this sentence held up logic for a long time. Here’s why. We
introduced the idea of referential semantics: language describes objects, and
some parts of language describe, while other parts some stand for, objects.

Now it’s not massively hard to think about how to generalize that idea to
account for words like ‘everybody’ or ‘somebody’. We simply say that something
like ‘Everybody golfs’ is true provided every object golfs. Think of it like
this: take everything, and go through them one by one. If every object we look
at is in the set of golfers, our sentence is true; if not, it is false. The same
goes for ‘somebody’: take all the objects, look through them one byone, and if
we find one that’s in the set of golfers, our sentence is true.

And it’s not so hard to generalize the account we gave of verbs to account for
transitive verbs. We just need to work out what object the sentence is talking
about, and how it is describing it. So consider ‘Obama loves Michelle’.

There are two things we could say: we could say that the bit that’s doing the
describing is ‘loves Michelle’ and the object described is Obama. Or we could
say that the bit doing the describing is ‘Obama loves’ and the object described
is Michelle. Either works: they’ll give the same truth condition (think about
that for a second to convince yourself).

But when we turn to 1, this ceases to be true. If we say that what’s doing the
describing is ‘loves somebody’ and the thing described is ‘everybody’, we’ll be
okay. But we could also take the object described as provided by ‘somebody’ and
‘everybody loves’ as doing the describing. But that yields a different reading:
it yields one on which somebody is such that everybody loves them. That’s a very
popular person.

The crucial point is that depending on how you break the sentence up, you get
different readings. Frege introduced a way to talk about such sentences to
account for this, the quantifier variable notion. It was part of his project to
introduce a scientifically precise language free from the ambiguities of natural
language, a project that was very influential at the start of the 20th century.
For now, let’s just introduce a bit of the language itself. Consider:

∃*y*∀*x *Loves(*y,x*)**∀*y*∃*x *Loves(*y,x*)

We read ∃*y* as saying ‘there exists an x such that’, and we read ∀*x* as saying
‘for all y’. These two formula correspond to different ways the sentence can be
broken up: the first corresponds to the reading on which ‘everybody loves’ is
doing the describing bit, while the second corresponds to the other reading.

In doing so, Frege was able to make sense of the fact that our sentence doesn’t
have a unique breakdown into object described and description. For now, the key
point is simply that Frege realized, and gave a way to deal with, this problem:
by associating a sentence with more than one logical formula. We’ll explore what
the symbols mean more below, but first let’s consider our second sentence.

(Let me just make something clear: expressions like the above, despite the
presence of the English-looking ‘Loves’, are not English. They are a separate,
formal language that we’re trying to use to regiment English and reveal its
underlying structure. I merely use English-looking expressions like ‘Loves’ to
make them easier to read.)


#### 2. The King of Ireland doesn’t exist (Russell, ‘On Denoting’)

Russell was very taken with the idea of referential semantics: with the thought
that words mean things in the world. Indeed, he thought that if a word didn’t
have such a worldly meaning — if there wasn’t something out there in the world
that it pointed to, the sentence was meaningless.

But that causes problems. Ireland doesn’t have a king, but the above sentence is
true (it sounds a bit unnatural, but you could imagine an ill-informed diplomat
saying that he met the kings of Norway, Holland, and Ireland, only to be told
‘you couldn’t have — the king of Ireland doesn’t exist’).

What that means is that we can’t treat ‘the king of Ireland’ as a name, as
simply standing for an object, because otherwise the sentence should be
meaningless. Russell’s thought was that should treat such sentences as general
sentences. In particular, he thought it meant the same as ‘it’s not the case
that there is one and only one King of France’. Translated, this looks like
(where ¬ translates ‘not’, A→B translates ‘if A then B’ and & translates … well
you can probably guess):

¬∃*x* KingOfIreland(*x*) & ∀*y* (KingOfIreland(*y*) → *x*=*y*).

Again, the exact detail of the translation doesn’t matter (though feel free to
try to figure out what that means and why). The key point is that by using the
sort of logical analysis Frege used, by looking at the sentence and trying to
clarify its underlying structure, Russell was able to use the philosophy of
language to guard himself against claims that referential semantics led one to
postulate all sorts of weird objects, like, for example, round squares (which
would be referred to by ‘the round square’). And he extended his theory to
account for names that cause similar problems by saying that a name like, for
example, ‘Pegasus’ is in fact a disguised definite description.

#### 3. This sentence is false (from antiquity)

You’ve probably heard this one before, but to see the problem with this
sentence, consider: for a sentence to be true, what it says must be true. So
assume sentence 3 is true, then what it says must be true. But it says sentence
3 is false, so assuming sentence 3 is true, sentence 3 is false. And likewise if
you assume it’s false. What we get is that if the sentence is true, it’s false,
and if it’s false, it’s true. And this is a contradiction according to most
systems of logic.

The liar sentence, of which 3 is an example, is a good test of philosophical
sensibility. You might think it’s a silly trick not worthy of attention, or you
might think it’s the sort of thing a life would be well-spent trying to resolve.
Personally, it took me about 7–8 years of studying philosophy before I moved
from the former to the latter camp.

Whatever your take, its importance in at least mathematical logic can’t be
denied: versions of something like it play a role in many of that discipline’s
greatest hits, like Goedel’s incompleteness theorem, Tarksi’s indefinability of
truth view, and it was Russell’s version of it for sets that put paid to Frege’s
goal of showing that mathematics was nothing over and above logic. Moreover,
work continues to this day to try to figure out what we should say about it: is
the sentence meaningless? Is it both true and false maybe? Or neither? There are
many options out there.

#### 4. ∃*x*Golfs(*x*) (Tarski, ‘The Concept of Truth In Formalized Languages’)

So far, we have introduced quantified sentences of a formal language, but we
haven’t said much about how they work. But there are deep problems here whose
resolution is our fourth high point of the philosophy of language.

We said that we could translate a sentence like ‘everybody golfs’ into ∀*x*
Golfs(*x*). A natural way to understand that is that we translate the
‘everybody’ bit into ∀*x* and the ‘golfs’ bit into ‘Golfs(*x*)’.

And that in turn would mean that ‘Golfs(x)’ in our artificial language functions
like ‘golfs’ in natural languages, as what I’ve called describing.

But how can this be? Because in our formal language ‘Golfs’ *by itself*
functions as a describing term. Are we to say that both ‘Golfs’ and ‘Golfs(x)’
have the same function despite their different form?

That would be awkward. Its awkwardness can be magnified when we note that
expressions containing ‘*x*’s can be as complicated as sentences. Just as we can
have sentences like the below (where v translates ‘or’):

Golf(Obama) & Sings(Obama) v ¬Dance(Obama)

So we can have

∃*x* Golfs(*x*) & Sings(*x*) v ¬Dance(*x*)

A moment’s reflection should reveal that expressions-containing-’x’s can have
all the same forms that sentences do. That suggests we’re missing an important
generalization by treating them as different types of thing.

So can we say they are sentences? Well, that seems difficult, for several
reasons. As already noted, we seem to want ‘Golfs(*x*)’ to function as a
describing expression, in particular as referring to the set of golfers. But
sentences aren’t describing expressions. Moreover, if it’s a sentence, just what
does the *x* stand for?

So have a problem: we want expressions like Golfs(*x*) to be both sentence-like
and description-like.

Tarski showed how to simultaneously satisfy these desiderata: how a formula like
Golfs(*x*) could be both sentence-like and verb-like. The basic thought is that
such formula are sentences, but only one you’ve specified a value of the ‘x’ .
They are sentences *relative to such a specification*. For example, a
specification is *x*=Beto; another is *x*=Cruz.

We can then say how quantifiers behave: a sentence like ∃*x* Golfs(*x*) is true
provided provided there is some specification of a value to *x* that makes
Golfs(*x*) come out true. A sentence like ∀*x* Golfs(*x*) is true provided for
every specification of a value to *x,* Golfs(*x*) comes out true.

To repeat, the clever idea is to introduce a parameter to make formulas like
Golfs(*x*) sentence-like enough to account for their distribution, but
property-like enough to reflect how they contribute to the meaning of sentences
in which they occur.

(The same thing applies in natural language. The key move here is to treat
pronouns like variables, and then roughly the same argument goes through. In
something like

Every man believes he is great

We treat — ignoring a few questions — ‘he is great’ as standing for a sentence
only relative to a choice of ‘*x*’.)

#### 5. Everybody golfs (Montague, ‘Proper Treatment of Quantification In Ordinary
English’)

Still on quantification! Things get subtle here, but the key point is quite
simple and can be simply made. Temporarily ignore everything above about
quantifiers and variables. Looking at our sentence 5 it certainly seems similar
to ‘John golfs’, doesn’t it? Traditional grammarians, for example, would say
that both consist of a subject and a predicate.

Now we know how to interpret ‘John golfs’. It’s true provided the reference of
John belongs in the reference of ‘golfs’. Could we possibly say the same thing
here?

Well, that seems difficult, because, as we’ve already noted, ‘everybody’ doesn’t
stand for any one object, but rather we use it when we want to check whether a
bunch of objects — all of them — are as the rest of the sentence describes them
to be.

So it seems hard to say that in 5 ‘everybody’ stands for something that ‘golfs’
describes. And so it seems like we’re going to have to give up the prima facie
attractive idea that sameness in subject-predicate form results in same
analysis.

But, in fact, we don’t. The insight of Frege that was first properly formalised
by Montague was that we can treat ‘everybody’ as if it describes the object
referred to by ‘golfs’. In particular, we can treat ‘everybody’ as describing
descriptions: it truly describes ‘golfs’ provided the property of golfing has
the property of being possessed by everyone (just as ‘runs’ truly describes
‘Obama’ provided Obama has the property of running). In set talk, we say that
‘everybody’ stands for a set of sets. A set is in this set provided all men are
members of it: that is to say, if it’s a property all men have.

This simple and clever idea enables us to treat, in a sense, ‘everybody golfs’
and ‘Obama golfs’ as involving the same semantic operations, a desirable result
in light of their similar form. And it generalizes to more complicated
construction, like ‘everybody loves someone’ and ‘every man thinks he is great’
but, with some regret, I will not describe how it does so here.

#### Interlude

If you’re still on-board, we’ve got pretty far. We’re now able to provide an
accurate semantic analysis of sentences containing quantifiers using just a few
rules. The key ideas are referential semantics, an account of meaning according
to which truth is the central concept, and an attempt to provide rules for how
the meaning of more complicated expressions gets built up by the meanings of the
parts of those expressions and how they are combined. In the next two sentences,
I want to consider some important ways in which this account of meaning must be
supplemented by something extra: a theory of how language is *used*.

#### 6. I thee wed (J.L. Austin, How To Do Things With Words)

Remember I said that we use language to describe the world. But that’s not all
we do with language. We also use language to *change* the word. Some actions are
such that the only way you can perform them is by saying something. When you say
things like that, you don’t describe some existing bit of reality, but rather
make it the case that a new bit of reality exists. When I utter 6 (in the
appropriate circumstance) I am not reporting on a preexisting bit of reality —
rather, I am making it the case that I am married to the person I am addressing.
These are known as ‘performative utterances’ and were made famous by J.L.
Austin, and the concept has proved very influential as showing the power of
language, and has been used, for example, in feminist analyses of gender and
pornography.

#### 7. She was rich but nice. (Grice ‘Logic and Conversation’)

Compare this sentence: ‘She was rich and nice’. Both these sentences make the
same demand on the world: that the person has both the properties of being rich
and of being nice. They are truth-conditionally equivalent. That means that, as
far as our theory of meaning is concerned, they are equivalent as to meaning.
But there is clearly something extra to 7 — it convey something over and above
its meaning. In particular, it conveys the attitude or prejudice on the part of
the speaker that rich people typically aren’t nice. Such conveyings, which are
over and above the meaning assigned by formal semantic theories, are called
‘implicatures’ by Grice, and again have been the object of much study. Together
6&7 form part of the domain of *pragmatics*, which is concerned, roughly, with
how we use language, particularly when that use enables us to do things that go
beyond what an expression’s literal meaning permits.

#### 8. It’s necessarily the case that 2+2=4 (Kripke, Naming and Necessity)

Remember we introduced ‘it is not the case that’ and treated it as if it were a
description that described sentences, and pointed out that treating the object
sentences described as truth values worked pretty well?

Well, its use is limited. To see this, consider the above sentence. It’s true,
right? If a sentence stands for a truth value, then any two sentences which
stand for the same truth value stand for the same thing. Now ‘2+2=4’ is true, as
is ‘grass is green’. So they stand for the same truth value. That means that
anything that truly describes what ‘2+2=4’ stands for truly describes what
‘grass is green’ stands for, because they stand for the same thing, and so that
means that because ‘it is necessarily the case that’ truly describes what
‘2+2=4’ stands for, it also truly describes what ‘grass is green’ stands for.

But it doesn’t, and what that suggests is that the account of sentence meaning
according to which sentences just mean truth values is no good.

Now, something like this observation dates back to Frege, and indeed you might
have thought even without any fancy philosophizing the meaning as truth value
stuff was weird and wrong.

But no one had a really formally good idea to deal with it before Kripke. On
Kripke’s view, a sentence has different truth values relative to different ways
the world could be (these ways are called ‘possible worlds’). ‘Grass is green’
stands for True relative to our world, but false relative to a possible world in
which grass is coal black. ‘2+2=4’, on the other hand, stands for true relative
to every world.

The useful idea is that we can treat ‘it’s necessary that’ as, in essence, a
universal quantifier that ranges over worlds, and so we can make use of our
logical understanding of quantifictional logic to account for things like
necessity and possibility and in general all environments like them (which
includes our talk about belief, knowledge, duty, and much else).

#### 9. I am here now (Kaplan, ‘Demonstratives’)

So thanks to Kripke, we now think that sentences are associated not with a
single truth value, but rather with a truth value for every possible world, and
we can use that to account for necessary truth (there’s a similar generalization
to be made for the meaning of subsentential expressions, but I won’t do so
here).

Now consider 9. There’s something kind of necessary-truth-like about it. Just as
‘2+2=4’ is always true in the sense that it’s true no matter what world you
consider it relative to, so ‘I am here now’ is always true in the sense that,
whenever uttered, it’s true.

So is it a necessary truth? No, obviously not. For me to say ‘I am here now’ is
to say Matt is in Northern Ireland on 10/11/2018. But that’s not necessarily
true. I could easily have been in France, for example.

In order, in part, to account for this notion of being always true when uttered
but not necessary, David Kaplan further complicated the Kripkean story. The
interesting thing about our sentence is that it contains *context-sensitive*
elements. That is, it contains elements whose reference differs depending on
where when and by whom they are uttered. The reference of ‘Obama’ doesn’t depend
on where, when, or by whom it is uttered. But ‘I’ does: in my mouth it means me,
Matt, in Obama’s mouth it means him, Obama. ‘Saturday 10th November 2018’
doesn’t depend on where, when, or by whom it is uttered, but ‘now’ does. Uttered
now, it stands for that Saturday. Uttered next Saturday, it stands for 17th
November 2018.

Now recall again Kripke: a sentence doesn’t have a truth value once and for all,
but rather has different truth values relative to different worlds. Call an
assignment of truth values to worlds like this a Kripke-meaning.

Kaplan’s thought is that an expression has a Kripke-meaning only relative to a
given context of utterance. A sentence like 9 is special because, no matter what
context it is uttered in, it expresses a sentence whose Kripke-meaning is true
relative to the world it is uttered in. This is complicated, and there’s no real
way to make it less so — you just have to think about it. But once you’ve read
it a few times you might be able to see it, and anyway the key point is that we
move from a picture first according to which sentences just mean truth values,
to one on which they truth values relative to worlds, to one on which they mean
truth values relative to worlds and contexts. The story keeps on getting more
complicated, but by doing so it becomes appeal to capture more data about how
language works.

#### Conclusion

We’ve covered a lot: about 100 years of sophisticated work and you’ve seen how
we’ve complicated our basic model to account for quantifiers, pronouns, modal
(like ‘it is necessary that’), performative and context-sensitive expressions.
That’s a lot! And work continues to this day in these and other areas, as we
build better and better theories to accommodate more and more data.

I would reiterate that understanding every detail is not completely necessary to
benefit from this post: if you understand the basic structure of the theory, and
the problems it should be sensitive to, then you now know roughly the aims and
methodology of much work in analytic philosophy of language.


