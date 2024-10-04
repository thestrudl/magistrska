# Master's Thesis: Evaluation of Emerging Free-to-Use VPN Solutions

This repository contains the LaTeX source files for my master's thesis, which addresses the evaluation of emerging VPN solutions in comparison to conventional VPN protocols.

## Abstract

In this thesis, we addressed emerging free-to-use VPN solutions. Lately, there are quite some new offerings on the VPN market, promising equal or better performance, security, and ease of use in comparison to conventional VPN solutions. We focused on the ZeroTier VPN solution, which works fundamentally differently from conventional VPNs as it uses SDN principles. Clients of a ZeroTier network authenticate on a server and then form a peer-to-peer network.

For the evaluation of VPN protocols, we designed a series of tests where we compared two emerging VPN solutions --- ZeroTier and WireGuard --- with two mature and established protocols --- OpenVPN and IKEv2/IPSec. The results of our testing showed that the most mature solution for industry use is **OpenVPN**. Meanwhile, **WireGuard** is a very efficient protocol with great potential.

## Project Structure

- `MagistrskaRV.tex`: Contains the LaTeX source code for the thesis.
- `fotografije/`: All images and graphs used in the thesis.
- `magistrska_viri_20220409.bib`: References and bibliography files.

## Usage

To compile the LaTeX files, you will need a LaTeX distribution installed on your system. You can compile the thesis by running:

Dependencies:
Pygments (on Mac `brew install Pygments`)
Inkscape (to render SVGs)

```bash
pdflatex --shell-escape MagistrskaRV.tex
bibtex MagistrskaRV.aux
pdflatex --shell-escape MagistrskaRV.tex §
pdflatex --shall-escape MagistrskaRV.tex #to fix the references
